<template>
  <div>
    <header class="m-header">
      <div class="m-header--logo">
        <menu-item link="/">
          <logo></logo>
        </menu-item>
      </div>
      <div class="m-header--sub">
        <menu-item link="/watch">Watch</menu-item>
        <menu-item link="/about">About</menu-item>
        <menu-item link="/press">Press</menu-item>
      </div>
    </header>
    <main>
      <router-view></router-view>
    </main>
    <footer class="m-footer">
      This site is not real. It is a site built for a class assignment in complete jest.
    </footer>
  </div>
</template>

<script>
import Logo from '@/components/Logo'
import MenuItem from '@/components/MenuItem'

export default {
  name: 'app',
  components: {
    'logo': Logo,
    'menu-item': MenuItem
  }
}
</script>

<style lang="scss">
.m-header {


  &--sub {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    margin-bottom: 1em;
  }
}

main {
  min-height: 40vh;
  max-width: 650px;
  margin: 0 auto;

  @media (min-width: 900px) {

    max-width: 85%;
  }
}

.m-footer {
  font-size: .75em;
  max-width: 760px;
  margin: 3em auto 2em;
  text-align: center;
}
</style>
