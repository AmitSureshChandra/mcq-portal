<template>
  <v-app dark>
    <v-app-bar fixed app> MCQ Mock Test </v-app-bar>
    <v-main>
      <v-container>
        <nuxt />
      </v-container>
    </v-main>

    <v-footer app>
      <span>&copy; {{ new Date().getFullYear() }} - built in nuxt </span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data() {
    return {};
  }
};
</script>
