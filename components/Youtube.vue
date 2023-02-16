<template>
  <lite-youtube class="flex-1" :videoid="id" params="autoplay=1" />
</template>
<script>
export default {
  props: {
    id: String,
    label: String,
  },
  fetchOnServer: false,
};
</script>
<style>
.flex-1 {
  flex: 1;
}
</style>
