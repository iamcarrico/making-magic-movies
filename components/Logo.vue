<template>
  <div class="m-logo">
    <img src="@/assets/making-magic-movies.png" class="m-logo-image">
    <div class="m-logo--text">Where the magic comes <strong>alive</strong>!</div>
  </div>
</template>

<script>
export default {
  name: 'logo'
}
</script>

<style lang="scss">
.m-logo {
  margin-top: 1em;
  max-width: 800px;

  &--text {
    font-style: italic;
    color: $green;
    text-align: center;
  }
}
</style>
