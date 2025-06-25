<template>
  <div class="container-fluid">
    <AppHeader />
    <AppMain></AppMain> <AppFooter />
  </div>
</template>

<script>
import AppHeader from './layouts/AppHeader.vue'
import AppFooter from './layouts/AppFooter.vue'
import AppMain from './layouts/AppMain.vue'
import '@/assets/css/style.css'

export default {
  name: 'BaseIndex',
  props: {
    msg: String
  },
  components: {
    AppHeader,
    AppFooter,
    AppMain
  }
}
</script>
