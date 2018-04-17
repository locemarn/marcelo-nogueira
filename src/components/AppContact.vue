<template>
  <v-card xs10 offset-xs1 sm8 offset-sm2 md6 offset-md3 id="form">
    <v-snackbar
      v-model="snackbar"
      absolute
      top
      right
      color="success"
    >
      <span>Message sent successfully!</span>
      <v-icon dark>check_circle</v-icon>
    </v-snackbar>
    <v-form @submit.prevent="submit" ref="form">
      <v-container grid-list-xl fluid>
        <v-layout wrap>
          <v-flex xs10 offset-xs1 sm8 offset-sm2 md6 offset-md3>
            <v-text-field
              color="teal"
              label="Name: "
              required
              v-model="form.name"
              :rules="rules.name"
            ></v-text-field>
          </v-flex>
          <v-flex xs10 offset-xs1 sm8 offset-sm2 md6 offset-md3>
            <v-text-field
              color="teal"
              label="Email: "
              v-model="form.email"
              required
              :rules="rules.name"
            ></v-text-field>
          </v-flex>
          <v-flex xs10 offset-xs1 sm8 offset-sm2 md6 offset-md3>
            <v-text-field
              color="teal"
              multi-line
              v-model="form.message"
            >
              <div slot="label">
                Message:
              </div>
            </v-text-field>
          </v-flex>
        </v-layout>
      </v-container>
      <v-card-actions>
        <v-spacer id="btn-contact">
        <v-btn
          fab
          outline
          color="teal"
          large
          right
          type="submit"
          :disabled="!formIsValid"
        ><v-icon dark>email</v-icon></v-btn>
        </v-spacer>
      </v-card-actions>
    </v-form>
  </v-card>
</template>

<script>
import Vue from 'vue'
import VueResource from 'vue-resource'

Vue.use(VueResource)

export default {
  data () {
    const defaultForm = Object.freeze({
      name: '',
      email: '',
      message: '',
      date: Date()
    })

    return {
      form: Object.assign({}, defaultForm),
      rules: {
        name: [val => (val || '').length > 0 || 'This field is required']
      },
      content: `Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer nec odio. Praesent libero. Sed cursus ante dapibus diam. Sed nisi. Nulla quis sem at nibh elementum imperdiet. Duis sagittis ipsum. Praesent mauris. Fusce nec tellus sed augue semper porta. Mauris massa. Vestibulum lacinia arcu eget nulla. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Curabitur sodales ligula in libero. Sed dignissim lacinia nunc.`,
      snackbar: false,
      terms: false,
      defaultForm
    }
  },

  computed: {
    formIsValid () {
      return (
        this.form.name &&
        this.form.email
      )
    }
  },

  methods: {
    resetForm () {
      this.form = Object.assign({}, this.defaultForm)
      this.$refs.form.reset()
    },
    submit () {
      this.$http.post('https://form-bc7e3.firebaseio.com/data.json', this.form).then(response => {
        this.nome = ''
        this.email = ''
        this.mensagem = ''
        this.snackbar = true
        this.resetForm()
      }, error => {
        console.error(error)
      })
    }
  }
}
</script>

<style>
/* #form {
  margin-top: 5%;
} */
</style>
