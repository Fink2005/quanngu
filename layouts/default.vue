<template>
  <v-app>
    <v-tool-bar class="d-flex justify-space-between mx-16 my-6">
        <v-tool-bar-title class="ml-14">
            <NuxtLink to=""><img src="https://cdn.prod.website-files.com/63877b2a41191ed2e132006b/64dff2526c35b16f4ec9b74e_Component%209.png" loading="lazy" width="124" alt=""></NuxtLink>
        </v-tool-bar-title>
        <div class="mr-14">
            <v-btn text rounded large class="text-capitalize">Organizations</v-btn>
            <v-btn text rounded large class="text-capitalize">Workers</v-btn>
            <v-menu rounded="xl" open-on-hover nudge-bottom="40" nudge-left="100">
                <template v-slot:activator="{ on, attrs }">
                    <v-btn text v-bind="attrs" v-on="on" rounded large class="text-capitalize">
                        <span>Resources</span>
                        <v-icon>mdi-chevron-down</v-icon>
                    </v-btn>
                </template>
                <v-card class="d-flex ma-4 pa-2" rounded="xl">
                    <div class="d-flex flex-column">
                        <v-list-subheader class="text-black text-bold font-weight-medium ml-8">Product</v-list-subheader>
                        <v-hover v-slot="{ hover }">
                            <v-btn rounded text class="text-capitalize text-body-2"><v-list-item :class="hover ? 'darkpurple--text' : 'darkgrey2--text'">FAQ</v-list-item></v-btn>
                        </v-hover>
                        <v-hover v-slot="{ hover }">
                            <v-btn rounded text class="text-capitalize text-body-2"><v-list-item :class="hover ? 'darkpurple--text' : 'darkgrey2--text'">Contact Us</v-list-item></v-btn>
                        </v-hover>
                    </div>
                    <v-divider class="mb-2"></v-divider>
                    <div class="d-flex flex-column">
                        <v-list-subheader class="text-black font-weight-medium ml-8">Other</v-list-subheader>
                        <v-hover v-slot="{ hover }">
                            <v-btn rounded text class="text-capitalize text-body-2"><v-list-item :class="hover ? 'darkpurple--text' : 'darkgrey2--text'">Terms & Conditions</v-list-item></v-btn>
                        </v-hover>
                        <v-hover v-slot="{ hover }">
                            <v-btn rounded text class="text-capitalize text-body-2"><v-list-item :class="hover ? 'darkpurple--text' : 'darkgrey2--text'">Privacy Policy</v-list-item></v-btn>
                        </v-hover>
                    </div>
                </v-card>
            </v-menu>
            <v-hover v-slot="{ hover }">
                <v-btn rounded :color="hover ? '#e4e6f1' : '#f89500'" depressed :dark="!hover" large class="text-capitalize">Get Started</v-btn>
            </v-hover>
        </div>
    </v-tool-bar>
    <v-main>
      <v-container class="pa-0 ma-0" fluid>
        <Nuxt />
      </v-container>
    </v-main>
    <v-sheet class="mt-16" width="100">
      <v-footer color="white" padless="false" absolute="false" class="d-flex align-center mt-16" width="100%" max-height="100%">
          <v-col class="d-flex align-center ml-9 mt-n16" col="12">
              <v-img class="" src="https://cdn.prod.website-files.com/63877b2a41191ed2e132006b/66309a5330883e87e23894ed_Component%2011.png" alt="" max-width="40"></v-img>
            <v-divider class="mx-4" vertical></v-divider>
              <p class="d-flex align-center font-weight-bold newgrey--text text--darken-1 caption">Copyright ©2024 JobInn Technologies Inc.</p>
          </v-col>
      </v-footer>
    </v-sheet>
  </v-app>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data () {
    return {}
  }
}

</script>

<style scoped>
  .v-menu__content {
    box-shadow: none;
  }
  .f-footer-line {
    background-color: #5e6672;
    width: 1px;
    height: 24px;
    margin-left: 16px;
    margin-right: 16px;
  }
</style>
