<template>
  <v-container id="max-width-container">
    <v-row class="ml-16 pl-6 d-flex flex-nowrap justify-space-around align-center mw-tc" height="600">
      <!-- Left Content -->
      <v-col cols="12" md="7" width="50%" id="width-col" class="d-flex flex-column align-start" >
        <div class="text-subtitle-2 font-weight-bold yellow--text text--darken-4 mb-4">WORKFORCE OF TOMORROW</div>
        <div class="font-weight-bold line-height">Train, Work, Hire: All in <span class="line-height font-weight-bold font-italic text-decoration-underline yellow--text text--darken-4">One</span></div>
        <div class="line-height font-weight-bold font-italic text-decoration-underline yellow--text text--darken-4">Place.</div>
        <div class="text-body-1 font-weight-medium mt-6">
          Train your community into a dynamic pool of skilled workers, ready to tackle one-off shifts seamlessly.
        </div>
        <v-hover v-slot="{ hover }">
          <v-btn :color= " hover ? '#dedfe3' : '#f69351' " :class="  hover ? 'black--text' : 'white--text' " class="mt-6 text-no-wrap rounded-pill text-subtitle-2 text-capitalize" style="width:150px; height:50px;">
            Get Started
          </v-btn>
        </v-hover>
      </v-col>
      <!-- Right Image -->
      <v-col cols="12" md="7" width="50%" id="max-width-img" class="d-inline-flex flex-column align-start ml-16 mt-16 pl-16 mr-n16">
        <v-img
          src="https://cdn.prod.website-files.com/63877b2a41191ed2e132006b/6611a6969d96ffefe01fbb94_Component%201.png"
          class="ml-16 pl-16"
      
        ></v-img>
      </v-col>
    </v-row>

    <!-- Bottom Section -->
    <v-row class="mt-16" justify="space-around">
      <v-col cols="12" md="6" lg="4" class="d-flex flex-column align-center mt-16">
        <v-img
          src="https://cdn.prod.website-files.com/63877b2a41191ed2e132006b/6630740717a94b73d8ed8dbc_star.svg"
          height="30"
          width="30"
        ></v-img>
        <div class="text-h5 font-weight-bold my-5">Organizations</div>
        <div class="text-center mb-5" style="max-width: 550px;">
          Meet your staffing needs with a reliable pool of trained professionals, ready for on-demand, short-term roles.
        </div>
        <div class="text-h6 font-weight-bold mt-4 yellow--text text--darken-3">Learn more</div>
      </v-col>

      <v-col cols="12" md="6" lg="4" class="d-flex flex-column align-center mt-16">
        <v-img
          class="ma-0"
          src="https://cdn.prod.website-files.com/63877b2a41191ed2e132006b/6630740717a94b73d8ed8dcd_receipt_long.svg"
          height="30"
          width="30"
        ></v-img>
        <div class="text-h5 font-weight-bold my-5">Workers</div>
        <div class="text-center mb-5" style="max-width: 550px;">
          Build skills and find flexible jobs. Work wherever and whenever you want, on your terms.
        </div>
        <div class="text-h6 font-weight-bold mt-4 yellow--text text--darken-3">Learn more</div>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'IndexPage',
}
</script>

<style>

.line-height {
  line-height: 90px !important;
  font-size : 4.75rem !important;
  letter-spacing: -0.0083333333em !important;
  font-family: "Claritycity", sans-serif !important;
  color: #00112b !important
}
#width-col {
  max-width: 570px
}
#max-width-img {
  max-width: 800px !important;
  height: auto !important;
  width: 100% !important
}
#max-width-container {
  max-width: 100% !important;
  max-height:100% !important
}
.mw-tc {
  max-width: 100% !important
}
</style>
