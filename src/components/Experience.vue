<template>
  <section class="timeline-section">
      <header class="text-center">
            <h1>Experience and Accolades</h1>
            <p>Put your creativity on the development highway</p>
        </header>
    <v-timeline :reverse="reverse">
      <v-timeline-item v-for="(data, i) in work_data" :key="i" :color="data.color">
        <span slot="opposite">{{ data.timeline }}</span>
        <v-card class="elevation-2" >
          <v-card-title class="text-h5">{{ data.title }}</v-card-title>
          <v-card-text v-html="data.desc">
          </v-card-text>
        </v-card>
      </v-timeline-item>

      <v-timeline-item v-for="(data, i) in school_data" :key="i" :color="data.color">
        <span slot="opposite">{{ data.timeline }}</span>
        <v-card class="elevation-2">
          <v-card-title class="text-h5" v-html="data.name"></v-card-title>
          <v-card-text v-html="data.certificate"> </v-card-text>
        </v-card>
      </v-timeline-item>
    </v-timeline>
  </section>
</template>

<script>
export default {
  data() {
    return {
      reverse: true,
      work_data: [
        {
          timeline: "2021 - present",
          title: "East African Data Handlers",
          color: 'red lighten-1',
          desc: "Work as a software engineer. Main roles are mobile development <br> with Flutter & Dart, building backend API's for web and mobile applications.",
        },
        {
          timeline: "2019 - 2021",
          title: "AleroGroup",
          color: 'red lighten-2',
          desc: "Main responsibilities were building web applications  as well as<br> UI/UX design of user interface. I also contirbuted in building backend API's for the web applications.",
        },
      ],

      school_data: [
        {
          timeline: "2016 - 2021",
          name: "Jomo Kenyatta University <br>of Agriculture and Technology",
          color: 'red lighten-3',
          certificate:
            "B.Sc. Computer Science. <br> Major - Software Engineering",
        },
        {
          timeline: "2016 (Feb - May)",
          name: "Zalego Institute of Technology",
          color: 'red lighten-4',
          certificate:
            "Software Development <br> - Major - Android Development (Java) <br> - Minor - Web Development",
        },
        {
          timeline: "2011 - 2015",
          name: "Meru School",
          color: 'red lighten-5',
          certificate:
            "Kenya Certificate of Secondary Education (K.C.S.E) <br> Mean Grade: B+",
        },
      ],
    };
  },
};
</script>

<style scoped>
header h1 {
  font-family: "Aboreto", cursive;
}

header p {
  font-family:"Silkscreen", cursive ;
}
.timeline-section {
  width: 50%;
  margin: 0 auto;
}
</style>