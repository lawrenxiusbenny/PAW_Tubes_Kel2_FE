<template>
  <div class="Dashboard">
    <v-app-bar color="white" dark app>
      <v-app-bar-nav-icon
        color="grey darken-3
"
        @click="drawer = !drawer"
      ></v-app-bar-nav-icon>
    </v-app-bar>

    <v-navigation-drawer
      :color="warna"
      class="fullheight"
      width="300px"
      v-model="drawer"
      app
    >
      <v-list-item>
        <v-list-item-content>
          <img src="@/assets/loogputih.png" alt width="60px" />
        </v-list-item-content>
      </v-list-item>
      <br />
      <v-list dense nav>
        <v-list-item
          v-for="item in items"
          :key="item.title"
          link
          tag="router-link"
          :to="item.to"
          class="text-xl-h1"
        >
          <v-list-item-content>
            <v-list-item-title style="color: #ffffff" class="pa-5">{{
              item.title
            }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item> </v-list
      ><br /><br /><br />
      <v-divider></v-divider>
      <v-btn text router @click="logout" class="white--text"
        ><v-icon color="white">mdi-power</v-icon>Logout</v-btn
      >
    </v-navigation-drawer>

    <!--<v-app-bar app fixed height="75px">
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
      <VSpacer />
      <v-toolbar-items> </v-toolbar-items>
    </v-app-bar>-->
    <div class="fullheight pa-5">
      <router-view></router-view>
    </div>
    <v-dialog v-model="dialog" max-width="400px">
      <v-card>
        <v-card-title>Do you sure want to logout ?</v-card-title>
        <v-card-actions>
          <v-spacer></v-spacer>
          <v-btn color="blue darken-2" @click="cancelLogout" class="mr-3 mb-5">No</v-btn>
          <v-btn color="grey" @click="logoutConfirm" class="mr-3 mb-5">Yes</v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>
  </div>
</template>
<script>
export default {
  name: "Dashboard",
  data() {
    return {
      dialog: false,
      drawer: true,
      warna: "#16294F",
      warnaText: "#ffffff",
      items: [
        { title: "Dashboard", to: "/admin-dashboard" },
        { title: "Man", to: "/admin/man" },
        { title: "Woman", to: "/admin/woman" },
        { title: "Accessories", to: "/admin/acc" },
      ],
    };
  },
  methods: {
    logout() {
      this.dialog = true;
    },
    logoutConfirm() {
      localStorage.removeItem("token");
      localStorage.removeItem("id");
      localStorage.removeItem("isLoggedIn");
      this.$router.push("/signIn");
    },
    cancelLogout() {
      this.dialog = false;
    },
  },
  mounted(){
    console.log(localStorage.getItem('token'));
  }
};
</script>
<style scoped>
.fullheight {
  min-height: 100vh !important;
}
.router {
  text-decoration: none;
  color: black;
}
</style>
