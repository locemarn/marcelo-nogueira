<template>
  <v-jumbotron :gradient="gradient" height="100%" style="margin-top: 1px;">
    <v-container align-content-center wrap>
      <v-layout wrap>
        <v-flex v-for="(item,index) in items" :key="index" sm5 offset-sm1>
          <v-card hover raised id="card" color="teal lighten-5" >
            <v-card-media>
              <img v-img:mygroup
                :src="item.src"
                v-img="{ title: item.title, description: item.description }"
                style="height: 200px; width: 100%"
              >
            </v-card-media>
            <v-card-title>
              <div>
                <span class="grey--text" v-text="item.title"></span><br>
                <span v-text="item.description"></span>
              </div>
            </v-card-title>
          </v-card>
        </v-flex>
      </v-layout>
    </v-container>
  </v-jumbotron>
</template>

<script>
export default {
  data: () => ({
    gradient: 'to top, #CCE8CB, #FFF',
    items: [
      {
        title: 'Blog',
        description: 'Blog made with laravel and Vue.js for learning the tools. The articles for now are fakers to see the reaction of the site. Soon I intend to put it on the air and write some interesting little things. :)',
        src: require('../assets/blog-02.png')
      },
      {
        title: 'Admin Blog',
        description: 'Administrative part of the Blog. Made with AdminLTE and configured by Laravel with access levels. Database used MYSQL.',
        src: require('../assets/blog-admin-01.png')
      },
      {
        title: 'E-commerce',
        description: 'E-commerce made following the udemy course "Complete Course of PHP 7". It was my first experience with php and I really enjoyed the result. Today I notice some items that can be improved, maybe who knows if it is for production.',
        src: require('../assets/2.png')
      },
      {
        title: 'E-commerce Admin area',
        description: 'Admin of e-commerce, also done with AdminLTE.',
        src: require('../assets/5.png')
      },
      {
        title: 'Web-Tap-Top',
        description: 'ABCR Web App for the control of concessionaires and carriers on the highways of the state of São Paulo.',
        src: require('../assets/6.png')
      },
      {
        title: 'Blog',
        description: 'Personal blog for technical topics about programming and some philosophies of life.',
        src: require('../assets/7.png')
      }
    ],
    dialog: false
  })
}
</script>

<style>
#card {
  margin: 5% auto;
  padding: 1%;
  width: 60%;
}
</style>

