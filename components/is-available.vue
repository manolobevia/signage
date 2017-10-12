<template>
    <span class="available" v-bind:class="{ unavailable: checkAvailability }"> available</span>
</template>

<script>

export default {
  computed: {
    checkAvailability () {
      return this.$store.state.laptops.locations[this.$route.params.location].device
    }
  },
  props: [
    'device'
  ]
}
</script>

<style lang="scss">

</style>
