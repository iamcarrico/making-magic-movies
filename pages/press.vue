<template>
  <div class="l-press">
    <h1>Press Releases</h1>
    <sub-menu>
      <menu-item link="/press/nov-1">November 1</menu-item>
    </sub-menu>

    <NuxtChild></NuxtChild>
  </div>
</template>

<script>
import MenuItem from '../components/MenuItem'
import SubMenu from '../components/SubMenu'

export default {
  name: 'press',
  components: {
    'menu-item': MenuItem,
    'sub-menu': SubMenu
  }
}
</script>

<style lang="scss">

.l-press {

}

</style>
