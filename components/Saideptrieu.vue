<template>  
  <v-sheet color="transparent" class="super-duper-box d-flex flex-column animate__animated animate__fadeIn">
      <v-sheet color="transparent" :class="$vuetify.breakpoint.mdAndDown ? flex-column : flex-row" class="super-box-1 d-flex ml-lg-16 justify-space-around" width="100%" height="100%">
        <v-sheet class="d-flex flex-column ml-lg-16" width="25%">
          <p class="pa1">
            FEATURES
          </p>
          <p class="pa2">
            Solve Your Staffing
          </p>
          <p class="pa3">
            Challenges
          </p>
          <p class="pa4">
            Our plateform provides tailored features that effortlessly address your staffing needs, ensuring the right talent is always ready for you.
          </p>
          <v-sheet class="but d-flex" justify="row">
            <v-hover v-slot="{ hover }">
              <v-btn class="btn1 text-capitalize white--text" 
              color="orange"
              :text="hover ? true : false" 
              rounded
              x-large>
              Get Started
              </v-btn>
            </v-hover>
            <p class="pa5">
              Try JobInn Today !
            </p>
          </v-sheet>
        </v-sheet>
        <v-sheet color="transparent" class="right d-flex flex-column mr-lg-16" width="40%" >
            <v-container class="big-c1 d-flex" >
             <v-card class="c1 ma-md-4 mr-lg-16 d-inline" outlined shaped elevation="3" >
                <div>
                  <img src="https://cdn.prod.website-files.com/63877b2a41191ed2e132006b/66307ea94b1a01a34c45b64b_public.svg" class="ma-md-4 ma-lg-4 mb-lg-0 elevation=1">
                </div>
                <v-card-title class="title1">
                  <h4>
                 Automated Smart <br> Matching
                  </h4>
                </v-card-title>
                <v-card-text>
                  Instantly connect with the perfect candidates for your needs.
                </v-card-text>
              </v-card>
              <v-card class="c2 ma-md-4" outlined shaped elevation="3" width="35%">
                <div>
                  <img src="https://cdn.prod.website-files.com/63877b2a41191ed2e132006b/66307ea94b1a01a34c45b631_offline_bolt.svg" class="ma-md-4 ma-lg-4 mb-lg-0">
                </div>
                <v-card-title class="title2">
                 Training and Badge  <br> Certification
                </v-card-title>
                <v-card-text>
                 Equip your workforce with specific skills, verified through certification.
                </v-card-text>
              </v-card>
            </v-container>
            <v-container class="big-c2 d-flex">
              <v-card class="c3 ma-md-4 mr-lg-16" outlined shaped elevation="3" width="35%">
                <div>
                  <img src="https://cdn.prod.website-files.com/63877b2a41191ed2e132006b/66307eaa4b1a01a34c45b653_password.svg" class="ma-md-4 ma-lg-4 mb-lg-0">
                </div>
                <v-card-title class="title3">
                  Compliance and Risk  <br> Management
                </v-card-title>
                <v-card-text>
                  Stay compliant with all employment laws and regulations.
                </v-card-text>
              </v-card>
              <v-card class="c4 ma-md-4" outlined shaped elevation="3" width="35%">
                <div>
                  <img src="https://cdn.prod.website-files.com/63877b2a41191ed2e132006b/66307ea94b1a01a34c45b622_timelapse.svg" class="ma-md-4 ma-lg-4 mb-lg-0">
                </div>
                <v-card-title class="title4">
                 Flexible Workforce  <br> Access
                </v-card-title>
                <v-card-text>
                  Access skilled on-demand workers to match your dynamic staffing needs.
                </v-card-text>
              </v-card>
            </v-container>
          </v-sheet>
        </v-sheet>
      <div class="super box 2">
      </div>
      <div class="down ma-md-0 mt-lg-16 d-flex">
          <v-sheet color="white" :class="$vuetify.breakpoint.mdAndDown ? flex-column : flex-row" class="d-flex justify-space-around">
            <v-sheet class="left-sheet ml-lg-16" height="100%" width="40%">
              <img src="https://cdn.prod.website-files.com/63877b2a41191ed2e132006b/6611aa9ef1eebb5a516fdf9b_figure.png">
            </v-sheet>
            <v-sheet class="right-sheet ml-lg-a" height="100%" width="40%">
              <p class="a">PAYMENT</p>
              <div class="all-3-line">
                <p class="b">Pay Only When You</p>
                <p class="c">Hire. No Hidden</p>
                <p class="d">Fees.</p>
              </div>
              <div class="d-flex flex-row">
              <v-sheet class="small-left-sheet c1 ma-md-4 mr-lg-16 ml-lg-0 ">
                <img src="https://cdn.prod.website-files.com/63877b2a41191ed2e132006b/66307de16383e5d5e177585c_star%20(1).svg">
                <p class="e">Workers Reliability</p>
                <p class="f">Insurance</p>
              </v-sheet>
              <v-sheet class="small-right-sheet c1 ma-md-4">
                <img src="https://cdn.prod.website-files.com/63877b2a41191ed2e132006b/66307de16383e5d5e177586e_payments.svg">
                <p class="g">Secure Payment</p>
                <p class="h">System</p>
              </v-sheet>
              </div>
              <p class="i">Only pay for results. With JobInn Corp, you're charged solely upon a successful hire — no hidden fees, just straightforward staffing solutions.</p>
              <v-sheet class="butt d-flex" justify="row">
            <v-hover v-slot="{ hover }">
              <v-btn class="btn2 text-capitalize white--text" 
              color="orange"
              :text="hover ? true : false" 
              rounded
              x-large>
              Get Started
              </v-btn>
            </v-hover>
            <p class="try">
              Try JobInn Today !
            </p>
            </v-sheet>
          </v-sheet>
            </v-sheet>
           
      </div>
  </v-sheet>

</template>
<script>
export default {
  name: 'Animated'
}
</script>
<style scoped>



.pa1{
   margin-top: 95px;
   letter-spacing: .08em;
    text-transform: uppercase;
    font-size: 16px;
    font-weight: 600;
    line-height: 1.8;
    font-family: Claritycity, sans-serif;
    color: #5e6672;
}
.pa2{
  font-size: 48px;
    font-style: normal;
    line-height: 1.2;
    font-family: Claritycity, sans-serif;
    font-weight: 700;
}
.pa3{
  font-size: 48px;
    font-style: normal;
    line-height: 1.2;
    font-family: Claritycity, sans-serif;
    font-weight: 700;
    padding-bottom: 0px;
}
.pa4{
  color: #00112b;
    letter-spacing: -.02em;
    margin-bottom: 0;
    font-size: 16px;
    line-height: 1.8;
    display: block;
    margin-block-start: 1em;
    margin-block-end: 1em;
    margin-inline-start: 0px;
    margin-inline-end: 0px;
    unicode-bidi: isolate;
    font-family: Claritycity, sans-serif;
    font-weight: 500;
    padding-top: 40px;
}
.but{
  display: flex;
  flex-direction: row;
  justify-content: left;
} 
.pa5{
  margin-top:15px;
  margin-left:20px;
}
.a{
letter-spacing: .08em;
    text-transform: uppercase;
    font-size: 16px;
    font-weight: 600;
    line-height: 1.8;
}
.b{
  font-size: 48px;
    font-style: normal;
    font-weight: 600;
    line-height: 1.2;
}
.c{
  font-size: 48px;
    font-style: normal;
    font-weight: 600;
    line-height: 1.2;
}
.d{font-size: 48px;
    font-style: normal;
    font-weight: 600;
    line-height: 1.2;}
.e{
  font-size: 16px;
    font-weight: 600;
    line-height: 1.8;
}
.f{
  font-size: 16px;
    font-weight: 600;
    line-height: 1.8;
}
.h{font-size: 16px;
    font-weight: 600;
    line-height: 1.8;}
.g{font-size: 16px;
    font-weight: 600;
    line-height: 1.8;}
.i{font-size: 16px;
  line-height: 1.8;
  letter-spacing: -.02em;}

.try{
  margin-top:15px;
  margin-left:20px;
  color: orange;
}
</style>
