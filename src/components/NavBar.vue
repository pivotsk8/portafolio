<template>
  <v-app-bar app color="black" dark flat class="px-12">
    <v-btn>
      <v-icon color="yellow" left class="mr-2">fas fa-signature</v-icon> rami portafolio
    </v-btn>
    <v-spacer></v-spacer>
    <v-btn text @click='scroll("home")' class="test-yellow">Home</v-btn>
    <v-btn text @click='scroll("bout ")' class="test-yellow">About</v-btn>
    <v-btn text @click='scroll("portafolio")' class="test-yellow">Portafolio</v-btn>
    <v-btn text @click='scroll("service")' class="test-yellow">Service</v-btn>
    <v-btn text @click='scroll("page")' class="test-yellow">Page</v-btn>
    <v-btn text @click='scroll("blog")' class="test-yellow">Blog</v-btn>
    <v-btn text @click='scroll("contact")' class="test-yellow">Contact</v-btn>
  </v-app-bar>
</template>

<script>
export default {
  methods: {
    scroll(refName) {
      const element = document.getElementById(refName);
      element.scrollIntoView({ behavior: "smooth" })

    },
  }
}
</script>

<style lang="scss" scoped></style>
