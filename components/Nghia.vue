<template>
  <v-app>
    <v-container id="max-width-container ml-16" fluid>
    <!-- Top Section -->
      <v-row class="d-flex align-center flex-nowrap justify-space-between mw-tc" :class="$vuetify.breakpoint.mdAndDown ? 'flex-column flex-wrap' : '' ">
      <!-- Left Content -->
        <v-col cols="12" md="6" class="d-flex flex-column" width="60%" :class="$vuetify.breakpoint.mdAndDown ? 'align-center text-center' : '' ">
          <div class="text-subtitle-2 font-weight-bold mb-4 sub-text">WORKFORCE OF TOMORROW</div>
          <div class="font-weight-bold line-height mb-4">
            Train, Work, Hire: All in <span class="font-weight-bold font-italic text-decoration-underline one-place-color">One Place</span>
          </div>
          <div class="text-body-1 font-weight-medium mt-6 text-body-width">
            Train your community into a dynamic pool of skilled workers, ready to tackle one-off shifts seamlessly.
          </div>
          <v-hover v-slot:default="{ hover }">
            <v-btn :color="hover ? '#dedfe3' : '#f89500'" :class="hover ? 'black--text' : 'white--text'" class="mt-6 text-no-wrap rounded-pill text-subtitle-2 text-capitalize" style="width:150px; height:50px;">
              Get Started
            </v-btn>
          </v-hover>
        </v-col>
      <!-- Right Image -->
        <v-col cols="12" md="6" class="d-flex justify-center mt-6" width="40%">
          <v-img src="https://cdn.prod.website-files.com/63877b2a41191ed2e132006b/6611a6969d96ffefe01fbb94_Component%201.png" class="responsive-img"></v-img>
        </v-col>
      </v-row>

    <!-- Bottom Section -->
      <v-row class="mt-16" justify="center" :class="$vuetify.breakpoint.mdAndDown ? 'flex-column flex-wrap' : '' ">
        <v-col cols="12" md="4" class="d-flex flex-column align-center text-center mt-16">
          <v-img src="https://cdn.prod.website-files.com/63877b2a41191ed2e132006b/6630740717a94b73d8ed8dbc_star.svg" height="30" width="30"></v-img>
          <div class="text-h5 font-weight-bold my-5">Organizations</div>
          <div class="text-center mb-5" style="max-width: 550px;">
            Meet your staffing needs with a reliable pool of trained professionals, ready for on-demand, short-term roles.
          </div>
          <div class="text-h6 font-weight-bold mt-4 yellow--text text--darken-3">Learn more</div>
        </v-col>

        <v-col cols="12" md="4" class="d-flex flex-column align-center text-center mt-16">
          <v-img src="https://cdn.prod.website-files.com/63877b2a41191ed2e132006b/6630740717a94b73d8ed8dcd_receipt_long.svg" height="30" width="30"></v-img>
          <div class="text-h5 font-weight-bold my-5">Workers</div>
          <div class="text-center mb-5" style="max-width: 550px;">
            Build skills and find flexible jobs. Work wherever and whenever you want, on your terms.
          </div>
          <div class="text-h6 font-weight-bold mt-4 yellow--text text--darken-3">Learn more</div>
        </v-col>
      </v-row>
    </v-container>
  </v-app>
</template>

<script>
export default {
  name: 'IndexPage',
}
</script>

<style scoped>
.line-height {
  line-height: 1.2 !important;
  font-size: 3.5rem !important;
  letter-spacing: -0.0083333333em !important;
  font-family: "Claritycity", sans-serif !important;
  color: #00112b !important;
  width: 100%;
  max-width: 400px;
}

#max-width-container {
  max-width: 100% !important;
  padding-left: 16px !important;
  padding-right: 16px !important;
}

.mw-tc {
  max-width: 100% !important;
}

.text-body-width {
  width: 100% !important;
  max-width: 470px !important;
}

.responsive-img {
  width: 100% !important;
  max-width: 750px !important;
  height: auto !important;
}

.sub-text {
  font-family: "Claritycity", sans-serif !important;
  color: #fbb040 !important;
}

.one-place-color {
  color: #f89500 !important;
}

@media (max-width: 960px) {
  .line-height {
    font-size: 2rem !important;
    line-height: 1.2 !important;
  }
}

@media (max-width: 600px) {
  .text-body-width {
    max-width: 300px !important;
  }
  .responsive-img {
    max-width: 400px !important;
  }
}

@media (max-width: 400px) {
  .text-body-width {
    max-width: 200px !important;
  }
  .responsive-img {
    max-width: 300px !important;
  }
}
</style>