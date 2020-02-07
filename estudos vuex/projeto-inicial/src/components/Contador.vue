<template>
    <div class="container">
      {{count}}
      <button @click="$store.commit('add')">Incrementar</button>
    </div>
</template>

<script>
export default {
  name: "Contador",
  computed: {
    count() {
      return this.$store.state.count;
    }
  }
};
</script>

<style>
</style>