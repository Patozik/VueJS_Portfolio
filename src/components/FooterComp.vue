<template>
  <v-footer dark padless>
      <v-card flat tile class="black white--text py-5 px-5 text-center" width="100%">
          <v-row>
            <v-col cols="12" sm="4">
                <v-card-text class="white--text pt-2">
                    <v-btn icon>
                        <v-icon @click="scroll('home')" color="#ff4d00">fa-motorcycle</v-icon>
                    </v-btn>
                </v-card-text>
            </v-col>
            <v-col cols="12" sm="4">
                <v-card-text class="pt-2">
                    <v-icon class="mx-2 white--text" size="32px" >mdi-facebook</v-icon>
                    <v-icon class="mx-2 white--text" size="32px" >mdi-twitter</v-icon>
                    <v-icon class="mx-2 white--text" size="32px" @click="openInNewTab('https://github.com/Patozik')" >mdi-github</v-icon>
                    <v-icon class="mx-2 white--text" size="32px" >mdi-instagram</v-icon>
                </v-card-text>
            </v-col>
            <v-col cols="12" sm="4">
                <v-card-text class="pt-2">
                    <v-btn class="mx-1 white--text" icon>
                        <v-icon color="#ff4d00">mdi-heart</v-icon>
                    </v-btn>
                    Created By Patryk Ozimina
                </v-card-text>
            </v-col>
          </v-row>
      </v-card>
  </v-footer>
</template>

<script>
export default {
    data: () => ({
        icons:[
            "mdi-facebook", "mdi-twitter", "mdi-github", "mdi-instagram"
        ]
    }),
    methods: {
        async openInNewTab(url) {
            window.open(url, '_blank').focus();
        },

        scroll(refName) {
            const element = document.getElementById(refName);
            element.scrollIntoView({behavior: "smooth"});
        } 
    }
}
</script>

<style>



</style>