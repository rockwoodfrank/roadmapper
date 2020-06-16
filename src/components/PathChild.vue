<template>
  <div class="path-child">
      {{ landmark.name }}
  </div>
</template>

<script>
export default {
    name: "PathChild",
    components: {
    },
    props: [`landmark`],
}
</script>

<style lang = "scss" scoped>
  .path-child {
    padding: 1em 2em;
    background-color: #bcdeff;
    border-radius: 0.5em;

    display: inline-block;
  }
</style>