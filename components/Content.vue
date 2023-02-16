<template>
  <v-col cols="12">
    <v-row no-gutters>
      <v-col cols="12" v-if="isShow.status == true" class="pc">
        <youtube id="0Es1n1lTq-w"> </youtube>
      </v-col>
      <v-col cols="12" v-if="isShow.status == false">
        <v-btn @click="isShow.status = !isShow.status">Test</v-btn>
      </v-col>
    </v-row>
  </v-col>
</template>
<script>
export default {
  props: {
    isShow: Object,
  },
};
</script>
