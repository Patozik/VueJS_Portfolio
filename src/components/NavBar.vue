<template>
    <v-app-bar app color="#1e1e1e" dark flat class="px-8">
        <v-btn icon>
            <v-icon @click="scroll('home')" large color="#ff4d00">fa-motorcycle</v-icon>
        </v-btn>
        <v-spacer></v-spacer>
        <v-btn text @click="scroll('home')">Home</v-btn>
        <v-btn text @click="scroll('about')">O Mnie</v-btn>
        <v-btn text @click="scroll('project')">Projekty</v-btn>
        <v-btn text @click="scroll('contact')">Kontakt</v-btn>
    </v-app-bar>
</template>

<script>
export default {
    methods: {
        scroll(refName) {
            const element = document.getElementById(refName);
            element.scrollIntoView({behavior: "smooth"});
        }
    }
}
</script>

<style>

</style>