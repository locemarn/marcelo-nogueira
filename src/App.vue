<template>
  <v-card height="200px" flat slider-color="purple lighten-3" >
    <v-bottom-nav  :value="true" :active.sync="e1" color="transparent">
      <v-btn flat color="teal" value="me">
        <span>Me</span>
        <v-icon>fas fa-user</v-icon>
      </v-btn>
      <v-btn color="teal" value="projects">
        <span>Projects</span>
        <v-icon>fa-briefcase</v-icon>
      </v-btn>
      <v-btn flat color="teal" value="contact">
        <span>Contact</span>
        <v-icon>fas fa-envelope</v-icon>
      </v-btn>
    </v-bottom-nav>
    <div class="headline text-xs-center" v-if="e1 === (value='me')">
      <AppMe></AppMe>
    </div>
    <div class="headline text-xs-center" v-else-if="e1 === (value='projects')">
      <AppProjects></AppProjects>
    </div>
    <div class="headline text-xs-center" v-else-if="e1 === (value='contact')">
      <AppContact></AppContact>
    </div>
  </v-card>
</template>

<script>
import AppMe from './components/AppMe.vue'
import AppProjects from './components/AppProjects.vue'
import AppContact from './components/AppContact.vue'

export default {
  data () {
    return {
      e1: 'me'
    }
  },
  components: {
    AppMe, AppProjects, AppContact
  }
}
</script>
