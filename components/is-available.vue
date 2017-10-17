<template>
    <span class="available" :class="{ unavailable: !count }"> available</span>
</template>

<script>

export default {
  props: [
    'count'
  ]
}
</script>

<style lang="scss">

</style>
