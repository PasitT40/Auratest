<template>
  <v-app>
    <v-main>
      <v-container fluid class="p-0">
        <Nuxt />
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: "DefaultLayout",
  data() {
    return {};
  },
};
</script>
<style>
.v-main {
  background-image: url("https://img95.lovepik.com/photo/40107/8354.gif_wh300.gif");
  background-size: cover;

  height: 100vh;
  padding: 0;
  margin: 0;
}
</style>
