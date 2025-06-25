<template>
  <AppHeader />
  <div class="base-index">
    <h1 class="font-bold text-2xl m-5">Base Index Component</h1>
    <p class="sub-title text-gray-600 m-5 ">{{ msg }}</p>
  </div>
  <AppFooter />
</template>

<script>
import AppHeader from './layouts/AppHeader.vue'
import AppFooter from './layouts/AppFooter.vue'

export default {
  name: 'BaseIndex',
  props: {
    msg: String
  },
  components: {
    AppHeader,
    AppFooter
  }
}
</script>
