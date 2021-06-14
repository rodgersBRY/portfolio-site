<template>
    <section>
        <header class="text-center">
            <h1>Let's Keep In Touch!</h1>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing.</p>
        </header>
        
        <form>
            <v-layout row justify-space-around class="form">
                <section>
                    <label for="name">Name:</label><br>
                    <input type="text" name="name" class="input mb-3" placeholder="Enter name">
                    <label for="name" class="mr-2">Email:</label>
                    <input type="text" name="name" class="input" placeholder="Enter Email">
                </section>
                <section>
                    <label for="name">Comments</label><br>
                    <textarea type="text" rows="5" name="name" class="input mb-3" placeholder="Write your Comments..." />
                    <v-btn type="submit" dark color="red darken-1" style="text-transform: capitalize;">Submit</v-btn>
                </section>
                <section class="location">
                    <p class="headline">Address:</p>
                    <p class="subtitle">Mawira Inc.</p>
                    <p class="subtitle">134 Stilla. Tae, 414515</p>
                    <p class="headline mt-2">Phone:</p>
                    <p class="subtitle">+254 712413243</p>
                </section>
            </v-layout>
        </form>
        
    </section>
</template>

<script>
export default {
    data() {
        return {

        }
    }
}
</script>

<style scoped>
.form {
    margin: 2rem 0;
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