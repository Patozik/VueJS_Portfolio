<template>
<!--HOME SECTION-->
<v-app id="home" class="homeView" :style="{ background: $vuetify.theme.themes.dark.background}">
<NavBar />
<v-container fluid>
  <v-row>
    <v-col cols="6">
      <v-img class="mainImg" src="mt_09_orange.png" contain max-height="500"></v-img>
    </v-col>
    <v-col cols="6" class="titleHello">
      <v-col offset-md="3">
        <v-img class="myPhoto" src="my_photo.jpg"></v-img>
      </v-col>
      <v-col class="titleDescription" md="9">
        <h3 class="orange--text text--darken-4 top">Cześć, jestem Patryk</h3>
        <h1 class="white--text">Programista</h1>
        <p class="description grey--text">
          Jestem absolwentem Karpackiej Państwowej Uczelni na kierunku Informatyka.<br /> 
          Oprócz ukończenia tego kierunku bardzo interesuję się informatyką w szczególności
          programowaniem, nowościami technologicznymi oraz motoryzacją. <br />
          Posiadam już spore doświadczenie w zawodzie, 
          ale również na stanowisku produkcyjnym. Bardzo szybko się uczę, lubię zdobywać 
          nowe doświadczenie, nie boję się podejmować nowych wyzwań.
        </p>
        <v-btn tile color="#ff4d00" dark>Dowiedz się więcej o mnie</v-btn>
      </v-col>
    </v-col>
    
<!--ABOUT SECTION-->
    
    <v-col id="about" cols="12" class="padd">
      <div class="first">
        <v-row>
          <v-col cols="12">
            <div class="child bgColor1">
              <v-icon color="#ff4d00" x-large class="ml-3">
                fa-earth-europe
              </v-icon>
              <h3 class="white--text ml-3 mt-4">Staż międzynarodowy</h3>
              <p class="grey--text ml-3 mt-6">
                Staż w Irlandi, Dublin
              </p>
              <v-btn color="#ff4d00" dark text>
                Zobacz więcej
                <v-icon right>mdi-arrow-right</v-icon>
              </v-btn>
            </div>
            <div class="child bgColor2">
              <v-icon x-large class="ml-3" dark>fa-certificate</v-icon>
              <h3 class="white--text ml-3 mt-4">Certyfikaty</h3>
              <p class="black--text ml-3 mt-6">
                Certyfikaty Cisco, Europass
              </p>
              <v-btn color="#1e1e1e" dark text>
                Zobacz więcej
                <v-icon right>mdi-arrow-right</v-icon>
              </v-btn>
            </div>
            <div class="child bgColor1">
              <v-icon color="#ff4d00" x-large class="ml-3">
                mdi-book-open-page-variant
              </v-icon>
              <h3 class="white--text ml-3 mt-4">Szkolenia</h3>
              <p class="grey--text ml-3 mt-6">
                Ukończone wiele kursów
              </p>
              <v-btn color="#ff4d00" dark text>
                Zobacz więcej
                <v-icon right>mdi-arrow-right</v-icon>
              </v-btn>
            </div>
          </v-col>
          <v-col cols="12" class="mt-10">
            <div class="child1 ">
              <h1 class="orange--text text--darken-4 mt-4 number">Technologie</h1>
              <h3 class="white--text mt-4">w których pracuje</h3>
            </div>
            <div class="child2 mRight">
              <v-row>
                <v-col cols="12" class="childcol">
                  <div class="child2 mButton padding bgColor1">
                    <v-icon color="#ff4d00" x-large class="iconAbout">
                      fa-brands fa-vuejs
                    </v-icon>
                    <p class="grey--text">Vue.JS</p>
                  </div>
                </v-col>
                <v-col cols="12" class="childcol">
                  <div class="child2 padding bgColor1">
                    <v-icon color="#ff4d00" x-large class="iconAbout">
                      fa-brands fa-node
                    </v-icon>
                    <p class="grey--text">Node.JS</p>
                  </div>
                </v-col>
              </v-row>
            </div>
            <div class="child2">
              <v-row>
                <v-col cols="12" class="childcol">
                  <div class="child2 mButton padding bgColor1">
                    <v-icon color="#ff4d00" x-large class="iconAbout">
                      fa-brands fa-html5
                    </v-icon>
                    <p class="grey--text">HTML 5</p>
                  </div>
                </v-col>
                <v-col cols="12" class="childcol">
                  <div class="child2 padding bgColor1">
                    <v-icon color="#ff4d00" x-large class="iconAbout">
                      fa-brands fa-css3
                    </v-icon>
                    <p class="grey--text">CSS 3</p>
                  </div>
                </v-col>
              </v-row>
            </div>
          </v-col>
        </v-row>
      </div>
    </v-col>

<!--PROJECT SECTION-->

    <v-col class="about" md="3" offset-md="3" id="project">
      <h4 class="white--text">WYBRANE PROJEKTY</h4>
      <p class="grey--text">Wykonane projekty</p>
    </v-col>
    <v-col md="3" class="about text-end">
      <v-btn tile color="#ff4d00" dark>Zobacz wszystkie</v-btn>
    </v-col>

    <div class="viewProject">
      <v-col cols="6">
        <v-col md="6" offset-md="6">
          <v-card class="pa-3 py-5" outlined tile color="#ff4d00">
            <v-img src="website_1.png" contain></v-img>
          </v-card>
        </v-col>

        <v-col md="6" offset-md="6">
          <v-btn color="white" dark text class="ml-n4">
            Projekt Śledzenie adresu IP
          </v-btn><br />
          <v-btn color="#ff4d00" dark text class="ml-n4">
            Zobacz więcej
            <v-icon right>mdi-arrow-right</v-icon>
          </v-btn>
        </v-col>
      </v-col>

      <v-col cols="6">
        <v-col md="6">
          <v-card class="pa-3 py-5" outlined tile color="#ff4d00" >
            <v-img src="website_2.png" contain></v-img>
          </v-card>
        </v-col>
        
        <v-col md="6">
          <v-btn color="white" dark text class="ml-n4">
            Projekt Pogoda w twoim mieście
          </v-btn><br />
          <v-btn color="#ff4d00" dark text class="ml-n4">
            Zobacz więcej
            <v-icon right>mdi-arrow-right</v-icon>
          </v-btn>
        </v-col>
      </v-col>
    </div>

<!--CONTACT SECTION-->

    <v-col cols="12" class="padd topInverse">
      <div class="second">
        <div class="secondchild1" id="contact">
          <v-row>
            <v-col cols="12">
              <h1 class="white--text">
                Jestem gotowy na realizację kolejnych projektów!
              </h1>
              <p class="grey--text">
                Kolejne projekty już wkrótce ...
              </p>
            </v-col>
          </v-row>
        </div>
      </div>
      <v-toolbar class="topTolbar" color="#111111" dark flat>
        <div class="secondBar">
          <v-btn text>Home</v-btn>
          <v-btn text>O Mnie</v-btn>
          <v-btn text>Projekty</v-btn>
          <v-btn text>Kontakt</v-btn>
        </div>
      </v-toolbar>
    </v-col>
  </v-row>
</v-container>
<FooterComp />
</v-app>
  
</template>

<script>
import NavBar from '@/components/NavBar.vue'
import FooterComp from '@/components/FooterComp.vue'

  export default {
    name: 'HomeView',

    components: {
    NavBar,
    FooterComp
},
  }
</script>

<style scoped>

@media only screen and (max-width: 959px) {
  .about {
    margin-left: 30px;
    margin-right: 30px;
  }
}

.homeView {
  min-width: 850px;
  margin-top: -80px;
}

.mainImg {
  margin-top: 120px;
}

.titleHello {
  margin-top: 90px;
}

.myPhoto {
  border-radius: 50%;
  width: 25%;
}

.titleDescription {
  margin-top: -30px;
}

.description {
  text-align: justify;
}

.top {
 margin-top: 10px;
}

.about {
  margin-top: -60px;
  padding-top: 100px;
}

.topInverse {
  margin-top: -250px;
}

.topTolbar {
  margin-top: 100px;
  text-align: center;
}

.iconAbout {
  margin: 10px 0;
}

.first {
  width: 100%;
  height: 610px;
  background: linear-gradient(
    to right,
    #181818,
    #181818 50%,
    #111111 50%,
    #111111 50%
  );
  text-align: center;
  padding: 2rem 2rem;
  margin-top: 40px;
}

.second {
  width: 100%;
  height: 400px;
  background: #181818;
  text-align: center;
  padding: 2rem 2rem;
}

.secondchild1 {
  display: inline-block;
  background-color: #1e1e1e;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: center;
  margin-top: 250px;
}

.child {
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: left;
  margin-right: 8px;
  margin-top: 10px;
  width: 245px;
}

.viewProject {
  width: 100%;
  display: inline-flex;
}

.bgColor1 {
  background-color: #1e1e1e;
}

.bgColor2 {
  background-color: #ff4d00;
}

.child1 {
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  margin-right: 5px;
  width: 240px;
}

.child2 {
  display: inline-block;
  width: 245px;
  vertical-align: middle;
}

.mRight {
  margin-right: 8px;
}

.mButton {
  margin-bottom: 8px;
}

.padding {
  padding: 8px 0px;
}

.col-12.padd {
  padding: 12px 0 !important;
}

.col-12.childcol {
  padding: 0 !important;
}

h1.number{
  font-size: 36px;
  font-weight: bold;
}

.secondBar {
  position: absolute; 
  margin-left: auto; 
  margin-right: auto; 
  left: 0; 
  right: 0; 
  text-align: center;
}

</style>