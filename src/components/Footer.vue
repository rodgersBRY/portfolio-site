<template>
    <footer class="footer">
        <v-layout row justify-space-around class="footer-links">
            <v-btn icon>
                <i class="bx bxl-instagram bx-md icons"></i>
            </v-btn>
            <v-btn icon>
                <i class="bx bxl-facebook bx-md icons"></i>
            </v-btn>
            <v-btn icon>
                <i class="bx bxl-linkedin bx-md icons"></i>
            </v-btn>
            <v-btn icon>
                <i class="bx bxl-github bx-md icons"></i>
            </v-btn>
        </v-layout>
        <v-layout justify-center align-center class="copyright pa-1 grey lighten-3">
            <p>copyright &copy; {{ year }} | All Rights Reserved</p>
        </v-layout>
    </footer>
</template>

<script>
export default {
    data() {
        return {
            year: ''
        }
    },

    created() {
        var dt = new Date()
        this.year = dt.getFullYear()
    }
}
</script>

<style scoped>
.footer-links {
    width: 40%;
    padding: 4rem;
    margin: 0 auto;
}
</style>