<template>
  <main></main>
</template>

<script>
export default {
  layout: "empty",
  beforeMount() {
    this.$router.push("/login");
  },
};
</script>

<style>
</style>