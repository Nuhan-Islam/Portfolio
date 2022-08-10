<template>
  <v-app
    id="home"
    :style="{ background: $vuetify.theme.themes.dark.background }"
  >
    <nav-bar />
    <v-container fluid>
      <v-row>
        <v-col cols="6">
          <v-img src="1.png" contain max-height="500"></v-img>
        </v-col>
        <v-col cols="6">
          <h1 class="yellow--text top">Nuhan Islam</h1>
          <h3 class="white--text">Fresh Graduate</h3>
          <p class="grey--text">
            A recent graduate with strong problem-solving skills, as well as excellent programming, development, and organizational skills. I wish to pursue a profession in the information technology field.<br />
            I'd like to work for a fast-growing company where I can contribute to its success while also honing my skills and knowledge.
          </p>
        </v-col>

        <v-col cols="12" class="padd">
          <div class="first" id="project">
            <v-row>
              <v-col cols="12">
                <div class="child bgColor1">
                  <h3 class="yellow--text ml-3 mt-4">Language</h3>
                  <p class="grey--text ml-3 mt-6">
                    C/C++ <br>
                    Java<br>
                    Python <br>
                  </p>
                </div>

                <div class="child bgColor2">
                  <h3 class="yellow--text ml-3 mt-4">Website Tool</h3>
                  <p class="grey--text ml-3 mt-6">
                    HTML<br>
                    CSS<br>
                    JavaScript<br>
                  </p>
                </div>
                
                <div class="child bgColor1">
                  <h3 class="yellow--text ml-3 mt-4">Database</h3>
                  <p class="grey--text ml-3 mt-6">
                    SQL<br/>
                    MySQL <br>
                    MongoDB
                  </p>
                </div>

                <div class="child bgColor2">
                  <h3 class="yellow--text ml-3 mt-4">Operating System</h3>
                  <p class="grey--text ml-3 mt-6">
                    Windows<br />
                    Linux <br>
                    MacOS
                  </p>
                </div>
              </v-col>
              <v-col cols="12" class="mt-10">
                <div class="child1">
                  <h3 class="yellow--text mt-4">Work Experience</h3>
                  <h1 class="red--text mt-4 ">4 Months</h1>
                  <h3 class="grey--text mt-4">Teacher Assistant <br> at AIUB</h3>
                  
                </div>
              </v-col>
            </v-row>
          </div>
        </v-col>
        <v-col md="3" offset-md="3" id="about">
          <h4 class="white--text mt-8">RELEVANT PROJECTS</h4>
        </v-col>
        <v-col md="3" class="text-end">
          <v-btn tile color="#A7121D" dark> View Details </v-btn>
        </v-col>
        <v-col md="3" offset-md="3">
          <v-card
            class="pa-2 py-12"
            outlined
            tile
            height="250px"
            color="#1E1E1E"
          >
            <v-img src="3.png" contain max-height=""></v-img>
          </v-card>
        </v-col>
        <v-col md="3">
          <v-card
            class="pa-2 py-12"
            outlined
            tile
            height="250px"
            color="#1E1E1E"
          >
            <v-img src="2.png" contain max-height=""></v-img>
          </v-card>
        </v-col>
        <v-col md="3" offset-md="3">
          <v-btn color="white" dark text class="ml-n4">Malicious Link Detection Using Web Analytics</v-btn
          ><br />

          <v-btn color="#A7121D" dark text class="ml-n4">
            Go to the project
            <v-icon right>mdi-arrow-right</v-icon>
          </v-btn>
        </v-col>
        
        
        
        
        
        <v-col cols="12" class="padd topInverse">
          <div class="second">
            <div class="secondchild1" id="contact">
              <v-row>
                <v-col cols="7">
                  <h3 class="white--text">
                    This website is at beginner level & under development
                  </h3>
                  <p class="grey--text">
                    I hope you like this.<br/>
                  </p>
                </v-col>
                <v-col cols="5">
                  <v-btn tile color="#A7121D" dark class="mt-16">
                    Send Mail
                  </v-btn>
                </v-col>
              </v-row>
            </div>
          </div>
          <v-toolbar class="topTolbar" color="#111111" dark flat>
            <div
              style="
                position: absolute;
                margin-left: auto;
                margin-right: auto;
                left: 0;
                right: 0;
                text-align: center;
              "
            >
              <v-btn text>LinkedIN</v-btn>
              <v-btn text>Facebook</v-btn>
              <v-btn text>Twitter</v-btn>
              <v-btn text> Instagram</v-btn>
            </div>
          </v-toolbar>
        </v-col>
      </v-row>
    </v-container>
    <Footer />
  </v-app>
</template>

<script>
import NavBar from "../components/NavBar.vue";
import Footer from "../components/Footer.vue";

export default {
  name: "Home",
  data: () => ({
    icons: ["mdi-facebook", "mdi-twitter", "mdi-linkedin", "mdi-instagram"],
  }),
  components: {
    NavBar,
    Footer,
  },
};
</script>
<style scoped>
.top {
  margin-top: 180px;
}
.topInverse {
  margin-top: -250px;
}
.topTolbar {
  margin-top: 100px;
  text-align: center;
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
  text-align: left;
  margin-top: 250px;
}
.child {
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: left;
  margin-right: 8px;
}
.bgColor1 {
  background-color: #1e1e1e;
}
.bgColor2 {
  background-color: #ce1d2a;
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
  padding: 8px 0;
}

.col-12.padd {
  padding: 12px 0 !important;
}
.col-12.childcol {
  padding: 0 !important;
}
h1.number {
  font-size: 50px;
  font-weight: bold;
}
</style>