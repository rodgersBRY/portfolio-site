<template>
  <div class="about">
    <header class="text-center">
      <h1>I Am Mawira, A Web & Mobile Developer</h1>
      <p>Life is too short for ordinary apps.</p>
    </header>
    <section class="cards">
      <v-layout row justify-space-around>
        <v-card
          flat
          width="350"
          height="200"
          color="white lighten-2"
          class="mx-4 my-10 text-center"
          v-for="(sk, i) in skills"
          :key="i"
        >
          <img
            v-if="sk.image"
            :src="sk.image"
            alt="responsive design"
            width="100%"
          >
          <v-icon v-else size="200" :color="sk.color">{{ sk.img }}</v-icon>
          <v-card-text class="grey lighten-2 pa-5">
            {{ sk.title }}
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
        {
          image: require("@/assets/responsive.png"),
          title: "Responsive Design",
          img: "mdi-desktop-mac",
          color: "blue darken-3",
        },
        {
          title: "JavaScript & JQuery",
          img: "mdi-language-javascript",
          color: "yellow darken-2",
        },
        {
          title: "HMTL5/CSS3",
          img: "mdi-language-html5",
          color: "orange darken-2",
        },
        { title: "Nuxt JS", img: "mdi-nuxt", color: "green lighten-2" },
        {
          title: "Flutter & Dart",
          img: "mdi-tablet-cellphone",
          color: "purple lighten-2",
        },
        { title: "Vue JS", img: "mdi-vuejs", color: "green lighten-2" },
        {
          title: "Material Design",
          img: "mdi-pencil-ruler",
          color: "blue lighten-2",
        },
        { title: "Node JS", img: "mdi-nodejs", color: "green lighten-2" },
        {
          title: "Python",
          img: "mdi-language-python",
          color: "yellow darken-2",
        },
      ],
    };
  },
};
</script>

<style scoped>
.cards {
  margin-top: 4rem;
}

header h1 {
  font-family: "Aboreto", cursive;
}

header p {
  font-family:"Silkscreen", cursive ;
}
</style>
