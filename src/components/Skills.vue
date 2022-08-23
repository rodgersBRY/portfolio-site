<template>
  <section class="skills">
    <header class="text-center">
      <h1>My Skills</h1>
      <p>Create, Curate, Teach. That's The Way I Code.</p>
    </header>

    <v-layout justify-space-around class="pa-4">
      <section class="programming">
        <p class="display-1">
          Programming <span style="font-weight: bolder;">Skills</span>
        </p>
        <p class="subtitle">
          I have an established knowledge in programming and here are some of
          the languages and frameworks I make use of.
        </p>
        <div class="skill-bars">
          <skill-bar :value="90" skill-name="HTML5/CSS3" />
          <skill-bar :value="90" skill-name="JavaScript" />
          <skill-bar :value="90" skill-name="VueJS" />
          <skill-bar :value="80" skill-name="Flutter & Dart" />
          <skill-bar :value="60" skill-name="Python" />
          <skill-bar :value="40" skill-name="NuxtJS" />
        </div>
      </section>
      <section class="design">
        <p class="display-1">
          Design <span style="font-weight: bolder;">Skills</span>
        </p>
        <p class="subtitle">
          Designing the user interface is the first step in developing something
          beautiful for the client.
        </p>
        <div class="skill-bars">
          <div class="d-flex">
            <v-progress-linear
              height="15"
              value="50"
              color="red"
              :buffer-value="percentage"
              class="my-2"
            />
            <p class="ml-3">Figma</p>
          </div>
        </div>
      </section>
    </v-layout>
  </section>
</template>

<script>
import Skillbar from "./skill_bar.vue";

export default {
  components: {
    "skill-bar": Skillbar,
  },
  data() {
    return {
      percentage: 100,
    };
  },
};
</script>

<style scoped>
.programming,
.design {
  width: 40%;
}

header :first-child {
  font-family: "Aboreto", cursive;
}

header p {
  font-family: "Silkscreen", cursive;
}
</style>
