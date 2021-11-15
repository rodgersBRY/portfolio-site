<template>
  <div class="home">
    <header class="nav-bar">
      <v-toolbar
        flat
        color="red lighten-2"
        light
        style="position: fixed; width: 100%; z-index: 1000"
      >
        <v-toolbar-title>
          <v-img
            :src="require('../assets/logo1.png')"
            alt="logo"
            max-width="200"
            max-height="100"
          ></v-img>
        </v-toolbar-title>

        <v-spacer />

        <div class="nav-links">
          <router-link
            tag="li"
            active-class="active"
            to="#home"
            v-scroll-to="'#home'"
            >Home</router-link
          >
          <router-link
            tag="li"
            active-class="active"
            to="#about"
            v-scroll-to="'#about'"
            >About Me</router-link
          >
          <router-link
            tag="li"
            active-class="active"
            to="#skills"
            v-scroll-to="'#skills'"
            >My Skills</router-link
          >
          <router-link
            tag="li"
            active-class="active"
            to="#portfolio"
            v-scroll-to="'#contact'"
            >My Portfolio</router-link
          >
          <router-link
            tag="li"
            active-class="active"
            to="#experience"
            v-scroll-to="'#contact'"
            >Experience</router-link
          >
          <router-link
            tag="li"
            active-class="active"
            to="#contacts"
            v-scroll-to="'#contact'"
            >Contacts</router-link
          >
        </div>
      </v-toolbar>
    </header>

    <main>
      <!-- image + text -->
      <header id="home">
        <v-img
          width="100%"
          height="700"
          :src="require('../assets/header.jpg')"
        ></v-img>
      </header>

      <section class="ux-geek">
        <h1>I Create Beautiful Responsive Websitss, Yes I am a UX Geek</h1>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Debitis fugit
          dicta voluptatem magni laudantium corrupti consequatur repudiandae.
          Libero soluta incidunt deleniti minus aspernatur ex perferendis
          laborum ea, maxime, molestias tempore temporibus magni minima,
          adipisci quibusdam? Eos, facilis rem amet molestiae impedit voluptatum
          distinctio sequi consequatur ducimus consectetur at quisquam repellat.
        </p>
      </section>

      <div id="about" class="about grey lighten-3">
        <AboutPage />
      </div>

      <article class="quote">
        <v-parallax
          :src="require('../assets/developer.jpeg')"
          height="400"
          class="parallax text-center"
        >
          <h1 style="font-size: 30px">
            If I asked People what they wanted, they would have said 'Faster
            Horses'
          </h1>
          <p class="subtitle" style="font-size: 20px">- Henry Ford</p>
        </v-parallax>
      </article>

      <div id="skills" class="Skills pa-10">
        <SkillsPage />
      </div>

      <div id="experience" class="experience grey lighten-3 pa-7">
        <Experience />
      </div>

      <div id="portfolio" class="portfolio grey lighten-3"></div>

      <div id="contact" class="contact grey lighten-3">
        <Contact />
      </div>

      <div class="footer">
        <Footer />
      </div>
    </main>
  </div>
</template>

<script>
export default {
  name: "Home",

  data() {
    return {};
  },
};
</script>

<style scoped>
.nav-links {
  margin-right: 4rem;
}

.nav-links li {
  display: inline-block;
  color: rgb(223, 215, 215);
  padding: 20px;
  margin: 0 15px;
}

.nav-links li:hover,
.nav-links li.active {
  color: white;
  cursor: pointer;
}

.ux-geek {
  width: 70%;
  margin: 5rem auto;
  text-align: center;
}

.about,
.contact {
  padding: 3rem 0;
}
</style>
