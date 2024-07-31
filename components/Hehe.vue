<template>
  <v-container>
    <div>
      <h4  class="text-h5 gay--text">CONTACT US</h4>
      <h2 class="text-h3 font-weight-bold" >Get in touch today</h2>
      <h5 class="subtitle-1">Reach out to us with any questions or feedback—our team is here to help you navigate your JobInn experience.</h5>
    </div>  
    <v-row>
        <v-col cols="12" md="6">
            <v-form ref="form" v-model="valid">
                <v-text-field
                v-model="name"
                :rules="[rules.required]"
                label="Name"
                required
                ></v-text-field>
          
                <v-text-field
                v-model="email"
                :rules="[rules.required]"
                label="Email"
                required
                ></v-text-field>
         
                <v-text-field
                v-model="phone"
                :rules="[rules.required]"
                label="Phone"
                required
                ></v-text-field>
         
                <v-text-field
                v-model="company"
                :rules="[rules.required]"
                label="Company"
                required
                ></v-text-field>

                <v-textarea
                v-model="message"
                :rules="[rules.required]"
                label="Leave us a message"
                required
                ></v-textarea>

                <v-btn class="white--text"
                color="#ffa84b"
                elevation="5"
                rounded
                >Send Message</v-btn>        
            </v-form>
        </v-col>

        <v-col cols="12" md="6">
            <v-card>
                <v-card-title>Contact details</v-card-title>
                    <v-list>
                        <v-list-item>
                          <v-list-item-content>
                            <v-list-item-title>Sales Team</v-list-item-title>
                            <v-list-item-subtile>sales@jobinn.io</v-list-item-subtile>
                          </v-list-item-content>
                        </v-list-item>
                    </v-list>

                    <v-list>
                        <v-list-item>
                          <v-list-item-content>
                            <v-list-item-title>Media Relations</v-list-item-title>
                            <v-list-item-subtile>media@jobinn.io</v-list-item-subtile>
                          </v-list-item-content>
                        </v-list-item>
                    </v-list>

                    <v-list>
                        <v-list-item>
                          <v-list-item-content>
                            <v-list-item-title>Help & Support</v-list-item-title>
                            <v-list-item-subtile>support@jobinn.io</v-list-item-subtile>
                          </v-list-item-content>
                        </v-list-item>
                    </v-list>
            </v-card>
        </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      name: '',
      email: '',
      phone: '',
      company: '',
      message: '',
      valid: false,
      rules: {
        required: (value) => !!value || 'Required.',
        email: (value) => /.+@.+\..+/.test(value) || 'E-mail must be valid.',
        phone: (value) => /^\(\d{3}\) \d{3} - \d{3}$/.test(value) || 'Phone must be valid.',
      },
    };
  },
  methods: {
    submit() {
      if (this.$refs.form.validate()) {
        // Handle form submission
        console.log('Form submitted');
      }
    },
  },
};
</script>

<style>

</style>