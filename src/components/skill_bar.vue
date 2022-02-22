<template>
  <div class="d-flex">
    <div class="bars" style="width: 80%">
      <v-progress-linear
        height="15"
        :value="value"
        color="red"
        :buffer-value="100"
        class="my-2"
      />
    </div>
    <p class="ml-3">{{ skillName }}</p>
  </div>
</template>

<script>
export default {
  name: "skillbar",
  props: {
    skillName: String,
    value: Number,
  },
};
</script>
