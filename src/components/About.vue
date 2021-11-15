<template>
  <div class="about">
    <header class="text-center">
      <h1>I am Mawira, a Web Designer & Developer</h1>
      <p>Life is too short for ordinary apps.</p>
    </header>
    <section class="cards">
      <v-layout row wrap justify-center>
        <v-card
        flat
        width="350"
        color="white lighten-2"
        class="mx-7 my-4 text-center"
        v-for="(sk, i) in skills"
        :key="i">
          <v-icon size="200">{{ sk.img }}</v-icon>
          <v-card-title>
            {{ sk.title }}
          </v-card-title>
          <v-card-text class="grey lighten-2 pa-5">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Officia expedita illo explicabo id.
          </v-card-text>
        </v-card>
      </v-layout>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      skills: [
        { title: "Responsive Design", img: "mdi-desktop-mac" },
        { title: "JavaScript & Jquery", img: "mdi-language-javascript" },
        { title: "HMTL5/CSS3", img: "mdi-language-html5" },
        { title: "React.JS", img: "mdi-react" },
        { title: "Vue.JS", img: "mdi-vuejs" },
        { title: 'Material Design', img: 'mdi-material-design' }
      ],
    };
  },
};
</script>

<style scoped>
.cards {
  margin-top: 4rem;
}
</style>
