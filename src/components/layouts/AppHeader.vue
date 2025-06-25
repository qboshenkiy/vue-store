<template>
  <header>
    <div class="logo">
      <img src="@/assets/image/logo.png" alt="My Vue Store" class="logo">
    </div>
    <nav>
      <router-link to="/">Home</router-link>
      <router-link to="/about">About</router-link>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'AppHeader'
}
</script>

<style scoped>
header {
  background-color: #f8f9fa;
  padding: 1rem;
}

nav {
  display: flex;
  gap: 1rem;
}
</style>
