<template>
  <section>
    <header class="text-center">
      <h1>Let's Keep In Touch!</h1>
      <p>Let all your ideas bloom. Then build the best app for your idea!</p>
    </header>

    <form>
      <v-layout row justify-space-around class="form">
        <section>
          <label for="name">Name:</label><br />
          <input type="text" name="name" class="input mb-3" />
          <label for="name" class="mr-2">Email:</label>
          <input type="text" name="name" class="input" />
        </section>
        <section>
          <label for="name" class="mr-2">Subject:</label>
          <input type="text" name="name" class="input mb-3" />
          <label for="name" class="mt-5">Message:</label><br />
          <textarea type="text" rows="5" name="name" class="input mb-5" />
          <v-btn
            type="submit"
            dark
            color="red darken-1"
            style="text-transform: capitalize;"
            >Submit</v-btn
          >
        </section>
        <section class="location">
          <p class="headline">Address:</p>
          <p class="subtitle">Mawira Corp.</p>
          <p class="subtitle">728 Nkubu, Meru. 60 200</p>
          <p class="headline mt-2">Phone:</p>
          <p class="subtitle">(+254) 712413243</p>
        </section>
      </v-layout>
    </form>
  </section>
</template>

<script>
export default {
  data() {
    return {};
  },
};
</script>

<style scoped>
.form {
  margin: 2rem 0;
}

header h1 {
  font-family: "Aboreto", cursive;
}

header p {
  font-family:"Silkscreen", cursive ;
}

.input {
  padding: 4px;
  border-radius: 5px;
  outline: none;
  color: grey;
  background: white;
  width: 100%;
  border: 1px solid grey;
}
</style>
