
<template>
  
  <v-sheet>
    <v-sheet  class="slider ">
      <h1 class="text-center py-10 text-h3 font-bold-black">Tailored for Your Needs</h1>
    <!-- v-tabs -->
    <v-tabs class="tabs animate__animated animate__fadeInUp"  slider-size="0" height="100px"  v-model="tab">
      <v-hover v-slot="{hover}">
      <v-tab :style="{'overflow' :hover ?'hidden' : 'none','transition' :hover ? '0.3s' : 'none', 'transform' :hover ? 'scale3d(1.06, 1.06, 1.01)' : 'none' }" class="tab ma-5 px-11 ml-16 rounded-xl black--text">Work</v-tab>

    </v-hover>
    <v-hover v-slot="{hover}">
      <v-tab :style="{'overflow' :hover ?'hidden' : 'none','transition' :hover ? '0.3s' : 'none', 'transform' :hover ? 'scale3d(1.06, 1.06, 1.01)' : 'none'}"  class="tab ma-5 px-11 rounded-xl black--text">Hire</v-tab>
    </v-hover>

    <v-hover v-slot="{hover}">
      <v-tab :style="{'overflow' :hover ?'hidden' : 'none','transition' :hover ? '0.3s' : 'none', 'transform' :hover ? 'scale3d(1.06, 1.06, 1.01)' : 'none' }"  class="tab ma-5 px-11 rounded-xl black--text">Both</v-tab>
    </v-hover>
        
    </v-tabs>

    <!-- v-tabs-items -->
    <v-tabs-items  class=" pa-10 animate__animated animate__fadeInUp" v-model="tab">
      <v-tab-item transition="fade-transition" class="itemNe pt-10">

        <v-card  id="card" class=" d-flex justify-space-between rounded-xl ">

          <v-card-title class="left">
            <v-container id="container-left">
              <h2>Work</h2>
              <p class=" font-weight-medium  text-sm-body-1">
                Be the Architect of Your Life. Work when you want, for whom you want, and maintain your independence.
              </p>
              <v-btn elevation="2" x-large class="warning rounded-lg">Learn more</v-btn>
            </v-container>
          </v-card-title>

          <v-text >
            <v-img width="425" class="rounded-r-xl" aspect-ratio="1" src="/img/anhne1.svg" alt="SVG Image"/>
            <v-img class="image " width="280" height="500" src="/img/anhne.png" alt="Image"/>
          </v-text>

        
        </v-card>


      </v-tab-item>
      <v-tab-item transition="fade-transition" class="itemNe pt-10">

        <v-card  id="card" class=" d-flex justify-space-between rounded-xl ">

          <v-card-title class="left">
            <v-container id="container-left">
              <h2>Hire.</h2>
              <p class=" font-weight-medium  text-sm-body-1">
                Overcome labour shortages by tapping into a flexible, dynamic workforce ready to contribute when you need them.
              </p>
              <v-btn elevation="2" x-large class="warning rounded-lg">Learn more</v-btn>
            </v-container>
          </v-card-title>

          <v-text >
            <v-img width="425" class="rounded-r-xl" aspect-ratio="1" src="https://cdn.prod.website-files.com/63877b2a41191ed2e132006b/6390598a314a2e88c1aa7e7d_marketing-team-card-bg-01.svg" />
            <v-img class="image " width="280" height="500" src="/img/phoneHire.png" alt="Image"/>
          </v-text>

         
        </v-card>


      </v-tab-item>
      <v-tab-item transition="fade-transition" class="both itemNe pt-10" >

        <v-card  id="card" class=" d-flex justify-space-between rounded-xl ">

          <v-card-title class="left">
            <v-container id="container-left-both">
              <h2>Both.</h2>
              <p class=" font-weight-medium  text-sm-body-1">
                Make Life Work for You. Hire help, or earn extra. JobInn connects you with opportunities for both.
              </p>
            </v-container>
          </v-card-title>

          <v-text >
            <v-img width="325" class="rounded-r-xl" aspect-ratio="1" src="https://cdn.prod.website-files.com/63877b2a41191ed2e132006b/6390599971afe7741f7faf63_design-team-card-bg-01.svg"  alt="SVG Image"/>
            <v-img class="imageBoth " width="280" height="500" src="/img/iphoneBoth.png" alt="Image"/>
          </v-text>
        </v-card>


      </v-tab-item>
    </v-tabs-items>
  </v-sheet>

    <v-sheet class="pt-16">
     
     
      <h1 class="text-center text-h3 font-bold-black animate__animated animate__fadeInUp">Our result in numbers</h1>
     
     
     
     
      <div class="number d-flex justify-center animate__animated animate__fadeInUp">
       
   
        <div class="number-item ">
          <div class="top d-flex justify-center">
            <h1>96</h1>
            <h1 class="orange--text">%</h1>
          </div>
          <div class="bottom">
            Customer satisfaction
          </div>
        </div>
   
        <div class="number-item">
          <div class="top d-flex justify-center">
            <h1>30</h1>
            <h1 class="orange--text">+</h1>
          </div>
          <div class="bottom">
            Organizations
          </div>
        </div>
   
        <div class="number-item">
          <div class="top d-flex justify-center">
            <h1>750</h1>
            <h1 class="orange--text">+</h1>
          </div>
          <div class="bottom text-center">
            Workers
          </div>
        </div>
   
        <div class="number-item">
          <div class="top d-flex justify-center">
            <h1>240</h1>
            <h1 class="orange--text">%</h1>
          </div>
          <div class="bottom">
            Company growth
          </div>
        </div>
      </div>


    </v-sheet>


  </v-sheet>
</template>

<script>
import 'animate.css'; // Import Animate.css

export default {

  data() {
    return {
      tab: 0 // Use 0 to initialize the first tab as active
    };
  }
};



</script>

<style scoped>



.tab {
  border: 1px solid transparent;
  width: 175px;
  max-height: 80px; 
  box-shadow:  0 2px 10px 0 rgba(0, 0, 0, 0.06);
}




.image { position: absolute; 
  top: -55px;
  right: 290px;
}
.imageBoth {
  position: absolute; 
  top: -55px;
  right: 200px;
}
h2 { max-width: 100px;}
.container {max-width: 10000px;}
#container-left {max-width: 300px;}
.itemNe {position: relative;}
.left { width:800px ;}
#card { box-shadow:  0 2px 10px 0 rgba(0, 0, 0, 0.06)}
p {max-width: 341px;}
.v-card__title {border-top-left-radius: 0 !important;
    border-top-right-radius: 0 !important; }

.both { padding-bottom: 100px !important;}
#container-left-both {max-width: 550px; padding-left: 150px;}
#container-left-both p { max-width: 380px;}
.number-item {padding: 50px;}
.number-item h1 {font-size: 70px;}
.bottom { font-size: 23px;
font-weight: 1000;}


.v-slide-group__content {padding: 7px;}


.v-tab {text-transform: capitalize ;}
.v-application .primary--text:hover { color: rgb(180, 56, 56) !important;
caret-color: rgb(191, 43, 43) !important; }

.tabs {padding-left: 310px;}



.animate__animated.animate__fadeInUp { --animate-delay: 1s;  --animate-duration: 2000ms;}
</style>
