<template>
  <v-app>
  <v-main>
    <v-container>
      <Nuxt />
    </v-container>
  </v-main>
  <v-footer color="white" padless="false" absolute="false" class="d-flex flex-row align-center">
    <v-col class="d-flex text-left" col="12">
      <img src="https://cdn.prod.website-files.com/63877b2a41191ed2e132006b/66309a5330883e87e23894ed_Component%2011.png" alt="" width="20" height="20"> </img>
      
      <p>Copyright ©2024 JobInn Technologies Inc.</p>
    </v-col>
  </v-footer>
</v-app>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data () {
    return {
    }
  }
}
</script>