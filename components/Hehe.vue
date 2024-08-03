<template>
  <v-container class="pb-16">
    <div>
      <v-row>
        <v-col cols="12" md="6">
          <v-form ref="form" v-model="valid">
            <v-row>
              <div>
                <h4 class="text-h5 nice--text font-weight-bold">CONTACT US</h4>
                <h2 class="text-h3 font-weight-bold">Get in touch today</h2>
                <h5
                  class="subtitle-1 haha--text"
                >Reach out to us with any questions or feedback—our team is here to help you navigate your JobInn experience.</h5>
              </div>
              <v-col cols="12" md="5">
                <div>
                  <p class="font-weight-bold">Name</p>
                  <v-text-field
                    v-model="name"
                    :rules="[rules.required]"
                    label
                    placeholder="John Carter"
                    required
                    dense
                    outlined
                    rounded
                  ></v-text-field>
                </div>
              </v-col>
              <v-col cols="12" md="5">
                <div>
                  <p class="font-weight-bold">Email</p>
                  <v-text-field
                    v-model="email"
                    :rules="[rules.required]"
                    label
                    placeholder="example@email.com"
                    required
                    dense
                    outlined
                    rounded
                  ></v-text-field>
                </div>
              </v-col>
              <v-col cols="12" md="5">
                <div>
                  <p class="font-weight-bold">Phone</p>
                  <v-text-field
                    v-model="phone"
                    :rules="[rules.required]"
                    label
                    placeholder="(123) - 456 - 789"
                    required
                    dense
                    outlined
                    rounded
                  ></v-text-field>
                </div>
              </v-col>
              <v-col cols="12" md="5">
                <div>
                  <p class="font-weight-bold">Company</p>
                  <v-text-field
                    v-model="company"
                    :rules="[rules.required]"
                    label
                    placeholder="Facebook"
                    required
                    dense
                    outlined
                    rounded
                  ></v-text-field>
                </div>
              </v-col>
            </v-row>

            <p class="font-weight-bold">Leave us a message</p>
            <v-textarea
              v-model="message"
              label
              placeholder="Please type your message here..."
              dense
              outlined
              rounded
            ></v-textarea>
            <v-sheet height="150px">
              <v-hover v-slot="{ hover }">
                <v-btn class="white--text px-8" height="70" :class="hover ? 'mt-0' : 'mt-5'" :color="hover ? 'haha' : '#ffa84b'" elevation="5" rounded="pill">Send Message</v-btn>
              </v-hover>
            </v-sheet>

          </v-form>
        </v-col>

        <v-col cols="12" md="6"> 
          <v-card class="rounded-xl">
            <div class="pl-16 pb-10">
              <v-card-title class="font-weight-bold">Contact details</v-card-title>
              <v-card-title
                class="haha--text"
              >Lorem ipsum dolor sit amet consectetur adipisc elit tortor eu egestas morbi sem vulputate.</v-card-title>
            </div>
            <v-list>
              <v-hover v-slot="{hover}">
               <div class="d-flex pl-16 pb-10" :style="{'transform' :hover ? 'translateX(10px)' :'none', 'transition' :hover ? '0.3s' :'none' }">
                <v-img
                  class="rounded-xl"
                  width="90px"
                  src="https://cdn.prod.website-files.com/63877b2a41191ed2e132006b/663a79fd197c66ccaaf0aa57_1.png"
                />
                <v-list-item>
                  <v-list-item-content>
                    <v-list-item-title class="font-weight-bold">Sales Team</v-list-item-title>
                    <v-list-item-subtile class="nice--text font-weight-bold">sales@jobinn.io</v-list-item-subtile>
                  </v-list-item-content>
                </v-list-item>
               </div>
              </v-hover>
            </v-list>

            <v-list>
              <v-hover v-slot="{hover}">
               <div class="d-flex pl-16 pb-10" :style="{'transform' :hover ? 'translateX(10px)' :'none', 'transition' :hover ? '0.3s' :'none'}">
                <v-img
                  class="rounded-xl"
                  width="90px"
                  src="https://cdn.prod.website-files.com/63877b2a41191ed2e132006b/663a7a9d0ab0fd1f9dcd27b7_2.png"
                />
                <v-list-item>
                  <v-list-item-content>
                    <v-list-item-title class="font-weight-bold">Media Relations</v-list-item-title>
                    <v-list-item-subtile class="nice--text font-weight-bold">media@jobinn.io</v-list-item-subtile>
                  </v-list-item-content>
                </v-list-item>
               </div>
              </v-hover>
            </v-list>

            <v-list>
              <v-hover v-slot="{hover}">
               <div class="d-flex pl-16 pb-10" :style="{'transform' :hover ? 'translateX(10px)' :'none', 'transition' :hover ? '0.3s' :'none'}">
                <v-img
                  class="rounded-xl"
                  width="90px"
                  src="https://cdn.prod.website-files.com/63877b2a41191ed2e132006b/663a7ab015cfd8386ed50986_3.png"
                />
                <v-list-item>
                  <v-list-item-content>
                    <v-list-item-title class="font-weight-bold">Help & Support</v-list-item-title>
                    <v-list-item-subtile class="nice--text font-weight-bold">support@jobinn.io</v-list-item-subtile>
                  </v-list-item-content>
                </v-list-item>
               </div>
              </v-hover>
            </v-list>
          </v-card>
        </v-col>
      </v-row>
    </div>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      name: "",
      email: "",
      phone: "",
      company: "",
      message: "",
      valid: false,
      rules: {
        required: value => !!value || "Required.",
        email: value => /.+@.+\..+/.test(value) || "E-mail must be valid.",
        phone: value =>
          /^\(\d{3}\) \d{3} - \d{3}$/.test(value) || "Phone must be valid."
      }
    };
  },
  methods: {
    submit() {
      if (this.$refs.form.validate()) {
        // Handle form submission
        console.log("Form submitted");
      }
    }
  }
};
</script>

<style scoped>
.v-btn{
  transition:  0.5s ease;
}
.show-btns {
  color: rgba(255, 255, 255, 1) !important;
}
</style>