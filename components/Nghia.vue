<template>
    <v-sheet class="d-flex flex-column justify-space-between ml-16 mt-16 mr-n16" color="transparent">
      <v-sheet class="d-flex justify-space-between">
        <!-- Left Content -->
        <v-sheet class="d-flex flex-column justify-center ml-16" style="width: 70%;">
          <div class="text-subtitle-2 font-weight-bold yellow--text text--darken-4 mb-4">WORKFORCE OF TOMORROW</div>
          <div class="text-h2 font-weight-black line-height" style="width: 400px;">Train, Work, Hire : All in</div>
          <div class="text-h2 font-weight-black font-italic text-decoration-underline yellow--text text--darken-4 pt-4">One Place.</div>
          <div class="text-body-1 mt-6" style="width: 500px;">
            Train your community into a dynamic pool of skilled workers, ready to tackle one-off shifts seamlessly.
          </div>
          <v-row>
            <v-col cols="12" md="3">
              <v-hover v-slot="{hover}">
                <v-btn :color="hover ? '#dedfe3' : '#f69351'" :class="hover ? 'black--text' : 'white--text'" class="pa-4 mt-6 text-no-wrap rounded-pill text-subtitle-2" style="width:150px; height:50px;">
                  Get Started
                </v-btn>
              </v-hover>
            </v-col>
          </v-row>
        </v-sheet>
        <!-- Right Image -->
          <v-sheet class="ml-16 mb-16">
           <v-img
            contain="true"
            background-position="right"
            class="ml-16 pl-16"
            lazy-src="https://cdn.prod.website-files.com/63877b2a41191ed2e132006b/6611a6969d96ffefe01fbb94_Component%201.png"
            style="width: 30%;"
            max-width="100%"
            src="https://cdn.prod.website-files.com/63877b2a41191ed2e132006b/6611a6969d96ffefe01fbb94_Component%201.png">
          </v-img>
          </v-sheet>
        </v-sheet>
  
      <!-- Bottom Section -->
      <v-sheet class="d-flex justify-space-around mt-16 mb-16">
        <v-sheet class="d-flex flex-column align-center mt-16">
          <v-img
            lazy-src="https://cdn.prod.website-files.com/63877b2a41191ed2e132006b/6630740717a94b73d8ed8dbc_star.svg"
            height="30"
            width="30"
            src="https://cdn.prod.website-files.com/63877b2a41191ed2e132006b/6630740717a94b73d8ed8dbc_star.svg">
          </v-img>
          <div class="text-h5 font-weight-bold mt-4">Organizations</div>
          <div class="text-center mt-4" style="width: 550px;">
            Meet your staffing needs with a reliable pool of trained professionals, ready for on-demand, short-term roles.
          </div>
          <div class="text-h6 font-weight-bold mt-4 yellow--text text--darken-3">Learn more</div>
        </v-sheet>
  
        <v-sheet class="d-flex flex-column align-center mt-16">
          <v-img
            lazy-src="https://cdn.prod.website-files.com/63877b2a41191ed2e132006b/6630740717a94b73d8ed8dcd_receipt_long.svg"
            height="30"
            width="30"
            src="https://cdn.prod.website-files.com/63877b2a41191ed2e132006b/6630740717a94b73d8ed8dcd_receipt_long.svg">
          </v-img>
          <div class="text-h5 font-weight-bold mt-4">Workers</div>
          <div class="text-center mt-4" style="width: 550px;">
            Build skills and find flexible jobs. Work wherever and whenever you want, on your terms.
          </div>
          <div class="text-h6 font-weight-bold mt-4 yellow--text text--darken-3">Learn more</div>
        </v-sheet>
      </v-sheet>
    </v-sheet>
  </template>
  
  <script>
  export default {
    name: 'IndexPage',
  }
  </script>
  
  <style>
  

  .line-height {
    line-height: 5px;
  }
  </style>
  