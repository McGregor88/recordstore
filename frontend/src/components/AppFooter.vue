<template>
  <v-footer height="auto" color="grey darken-4">
    <v-layout justify-center row wrap>
      <v-btn v-for="link in links" :key="link" color="white" flat>{{ link }}</v-btn>
      <v-flex teal lighten-1 py-3 text-xs-center white--text xs12>
        &copy;{{ new Date().getFullYear() }} —
        <strong>Recordsore</strong>
      </v-flex>
    </v-layout>
  </v-footer>
</template>

<script>
export default {
  data: () => ({
    links: ["Home", "About Us", "Team", "Services", "Blog", "Contact Us"]
  })
};
</script>

<style lang="sass">
</style>