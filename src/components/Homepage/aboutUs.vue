<template>
  <div>
    <navbar-component></navbar-component>
    <div class="backs">
      <!-- <v-img :src="require('@/assets/fashion.jpg')" class="d-block w-100" alt="aboutPic" max-height="700"></v-img> -->
      <v-row align="center" justify="center"> </v-row>
      <hr style="height: 200pt; visibility: hidden" />
      <div align="center">
        <h4></h4>
        <br />
        <h1 class="white--text" style="font-size: 4em; justify-content: center">
          Get your style FASTER
        </h1>
        <h3 class="white--text" style="font-size: 4em; justify-content: center">
          and BETTER with us
        </h3>
        <br />
        <div class="my-2" align="center" justify="center">
          <v-btn depressed class="black white--text" href="#section2"
            >Learn About Us</v-btn
          >
        </div>
      </div>
      <hr style="height: 200pt; visibility: hidden" />
    </div>
    <template>
      <v-container grid-list-md id="section2">
        <v-card shaped flat class="text-center ma-3">
          <v-card-title bold class="justify-center">
            <div style="color: black; font-weight: bold">
              We believe that fashion can give people more confidence
            </div>
          </v-card-title>
          <v-card-subtitle>
            <div style="color: grey">
              <br />OLEH's Style opened in September of 2020 as a concept store to
              <br />provide the latest fashion trends from around the globe under one roof
              at an affordable price. <br />We offer fashion, design and services that
              enable people to be inspired and to express their own personal style
            </div>
          </v-card-subtitle>
        </v-card>
        <!-- <v-container>
                        <v-row>
                            <v-col lg="3" md="4" sm="6">
                                <v-card class="mb-2" tile="">
                                    <v-row align="start">
                                        <v-col class="shrink">
                                            <v-img :src="require('@/assets/fashion.jpg')" alt="..." style="width: 300px; height: 200px;"></v-img>
                                        </v-col>
                                        <v-col>
                                            <v-card-title class="pa-0"><div style="color:black;font-weight: bold;">LOCATION</div></v-card-title>
                                            <v-card-subtitle><div style="color: black;">
                                                Our company has spread all over the world,
                                                more than 50 branches and our first 
                                                company is in the capital city of Indonesia,
                                                Jakarta. Not just that but we also planning to
                                                spread our company in 4 other countries
                                                around the world
                                            </div></v-card-subtitle>
                                        </v-col>
                                    </v-row>
                                </v-card>
                            </v-col>
                        </v-row>
                    </v-container> -->
                    
        <v-container fluid>
          <v-layout justify-space-around>
            <v-flex xs5>
              <v-layout column>
                <br />
                <v-card shaped flat class="text-left ma-3">
                  <v-col class="shrink">
                    <!-- <v-img
                      :src="require('@/assets/maps.png')"
                      alt="..."
                      height="265"
                    ></v-img> -->
                    <Map />
                  </v-col>
                  <br />
                  <v-col>
                    <v-card-title bold class="justify-left">
                      <div style="color: black; font-weight: bold">How We Started</div>
                    </v-card-title>
                    <v-card-subtitle>
                      <div style="color: grey">
                        In the first of 2020 we start a small group to sell products about
                        fashion, and we consider our group can be developed to be a
                        company. And then we start to spread our company all over the
                        world until now, our company is still growing.
                      </div>
                    </v-card-subtitle>
                  </v-col>
                </v-card>
              </v-layout>
            </v-flex>
            <v-flex xs5>
              <v-layout column>
                <v-card shaped flat class="text-left ma-3">
                  <v-col>
                    <br /><br />
                    <v-card-title bold class="justify-left">
                      <div style="color: black; font-weight: bold">LOCATION</div>
                    </v-card-title>
                    <v-card-subtitle>
                      <div style="color: grey">
                        Our company has spread all over the world, more than 50 branches
                        and our first company is in the capital city of Indonesia,
                        Jakarta. Not just that but we also planning to spread our company
                        in 4 other countries around the world
                      </div>
                    </v-card-subtitle>
                  </v-col>
                  <br /><br /><br />
                  <v-col class="shrink">
                    <v-img
                      :src="require('@/assets/started.jpg')"
                      alt="..."
                      height="265"
                      width="400"
                    ></v-img>
                  </v-col>
                </v-card>
              </v-layout>
            </v-flex>
          </v-layout>
        </v-container>
        <br /><br /><br />
        <v-row class="d-flex justify-space-around mb-6">
          <v-card shaped style="background-color: whitesmoke; width: 270px; height: 350px">
            <v-card-title style="font-weight: bold; color: gray">
              <h2 style="color: #4f4f4f">Style Idea</h2>
            </v-card-title> 
            <v-card-subtitle style="color: grey">
              <h6>We continue to develop our designs to be the best and comfortable to wear.
              The ideas of our designs come from research in various countries. We also
              invite design experts to develop our products.</h6>
            </v-card-subtitle>
          </v-card>

          <v-card shaped style="background-color: whitesmoke; width: 270px; height: 350px">
            <v-card-title style="font-weight: bold; color: gray">
              <h2 style="color: #4f4f4f">Comfy to Wear</h2>
            </v-card-title>  
            <v-card-subtitle style="color: grey">
              <h6>We combine the designs and materials we collect to make a product that is
              comfortable to wear. We also organize all of our products into sections, so
              that you can choose our products according to your wishes.</h6>
            </v-card-subtitle>
          </v-card>

          <v-card shaped style="background-color: whitesmoke; width: 270px; height: 350px">
            <v-card-title style="font-weight: bold; color: gray">
              <h2 style="color: #4f4f4f">Cheap Prices</h2>
            </v-card-title>
            <v-card-subtitle style="color: grey">
              <h6>Beside we develop our products with the best material and the best design we
              also selling our products with low prices. Why? we really care people's
              fashion nowadays and we believe we produce the best fashion all over the
              world.</h6>
            </v-card-subtitle>
          </v-card>
        </v-row>
        <br /><br />
        <v-card shaped flat class="text-center ma-3">
          <v-card-title bold class="justify-center">
            <div style="color: black; font-weight: bold">
              "Fashion you can buy, but style you possess.
              <br />The key to style is learning who you are, which takes years.
              <br />There's no how-to road map to style. It's about self expression and,
              above all, attitude."
            </div>
          </v-card-title>
          <v-card-subtitle>
            <div style="color: grey"><br />- Iris Apfel</div>
          </v-card-subtitle>
        </v-card>
      </v-container>
    </template>
    <footer-component></footer-component>
  </div>
</template>
<script>
import Map from './Map';
import Header from "../Navbar.vue";
import Footer from "../Footer.vue";
export default {
  name: "aboutUs",
  components: {
    "navbar-component": Header,
    "footer-component": Footer,
    Map
  },
};
</script>

<style scoped>
.backs {
  background-image: url(../../assets/fashion.jpg);
  background-attachment: fixed;
  background-size: cover;
  position: center;
  background-repeat: no-repeat;
}
html {
  scroll-behavior: smooth;
}
</style>
