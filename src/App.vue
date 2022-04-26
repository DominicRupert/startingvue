<template>
  <header>
    <Navbar />
  </header>
  <main>
      <h1>{{ name }}</h1>
    <router-view />
  </main>
  <footer>
    <div class="bg-dark text-light text-center p-4">
    </div>
  </footer>
</template>

<script>
import { computed } from 'vue'
import { AppState } from './AppState'
export default {
  name: '',
  setup() {
    return {
      name: "Dom",
      appState: computed(() => AppState)
    }
  }
}
</script>
<style lang="scss">
@import "./assets/scss/main.scss";

</style>
