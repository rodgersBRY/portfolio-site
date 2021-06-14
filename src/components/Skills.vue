<template>
    <section class="skills">
        <header class="text-center">
            <h1>My Skills</h1>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing.</p>
        </header>

        <v-layout justify-space-around class="pa-4">
            <section class="programming">
                <p class="display-1">Programming <span style="font-weight: bolder;">Skills</span></p>
                <p class="subtitle">Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda suscipit iste consequuntur temporibus libero fuga quis sint ad sed!</p>
                <div class="skill-bars">
                    <div class="d-flex">
                        <v-progress-linear height="15" value="90" color="red" :buffer-value="percentage" class="my-2" />
                        <p class="ml-3">HTML5/CSS3</p>
                    </div>
                    <div class="d-flex">
                        <v-progress-linear height="15" value="90" color="red" :buffer-value="percentage" class="my-2" />
                        <p class="ml-3">JavaScript</p>
                    </div>
                    <div class="d-flex">
                        <v-progress-linear height="15" value="30" color="red" :buffer-value="percentage" class="my-2" />
                        <p class="ml-3">React.JS</p>
                    </div>
                    <div class="d-flex">
                        <v-progress-linear height="15" value="80" color="red" :buffer-value="percentage" class="my-2" />
                        <p class="ml-3">Vue.JS</p>
                    </div>
                </div>
            </section>
            <section class="design">
                <p class="display-1">Design <span style="font-weight: bolder;">Skills</span></p>
                <p class="subtitle">Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda suscipit iste consequuntur temporibus libero fuga quis sint ad sed!</p>
                <div class="skill-bars">
                    <div class="d-flex">
                        <v-progress-linear height="15" value="50" color="red" :buffer-value="percentage" class="my-2" />
                        <p class="ml-3">Figma</p>
                    </div>
                </div>
            </section>
        </v-layout>
    </section>
</template>

<script>
export default {
    data() {
        return {
            percentage: 100,
        }
    }
}
</script>

<style scoped>

.programming,
.design {
    width: 40%;
}


</style>