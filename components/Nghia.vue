<template>
  <v-container>
    <v-row class="d-flex justify-space-between mt-16 align-center">
      <!-- Left Content -->
      <v-col cols="12" md="7">
        <div class="text-subtitle-2 font-weight-bold yellow--text text--darken-4 mb-4">WORKFORCE OF TOMORROW</div>
        <div class="text-h2 font-weight-bold line-height">Train, Work, Hire: All in</div>
        <div class="text-h2 font-weight-bold font-italic text-decoration-underline yellow--text text--darken-4 pt-4">One Place.</div>
        <div class="text-body-1 font-weight-medium mt-6">
          Train your community into a dynamic pool of skilled workers, ready to tackle one-off shifts seamlessly.
        </div>
        <v-btn color="#f69351" class="pa-4 mt-6 text-no-wrap rounded-pill text-subtitle-2" style="width:150px; height:50px;">
          Get Started
        </v-btn>
      </v-col>
      <!-- Right Image -->
      <v-col cols="12" md="5">
        <v-img
          aspect-ratio="16/9"
          src="https://cdn.prod.website-files.com/63877b2a41191ed2e132006b/6611a6969d96ffefe01fbb94_Component%201.png"
          class="ml-md-16 pl-md-16"
          max-width="100%"
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
        <div class="text-h5 font-weight-bold mt-4">Organizations</div>
        <div class="text-center mt-4" style="max-width: 550px;">
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
        <div class="text-h5 font-weight-bold mt-4">Workers</div>
        <div class="text-center mt-4" style="max-width: 550px;">
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
.v-image__image--cover {
  background-size: contain !important
}
.line-height {
  line-height: 5px;
}
</style>
