<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  components: {
    AppHeader,
    AppMain,
    AppFooter
  }
}

</script>

<template>
  <div>
    <header>
      <AppHeader />
    </header>
    <main>
      <AppMain />
    </main>
    <footer>
      <AppFooter />
    </footer>
  </div>

</template>

<style lang="scss">
@use './styles/generals.scss'

</style>
