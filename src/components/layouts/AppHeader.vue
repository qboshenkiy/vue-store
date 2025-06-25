<template>
  <header>
    <div class="flex btw gp-1 header-container">
      <div class="logo flex gp-1">
        <img src="@/assets/image/logo.png" alt="My Vue Store" class="logo" />
        <div class="logo-container">
          <h1 class="logo-title">VUE SNEAKERS</h1>
          <p class="logo-subtitle">Магазин лучших кроссовок</p>
        </div>
      </div>
      <nav>
        <ul class="nav-list flex gp-1">
          <li>
            <a href="/" class="link-nav">
              <img src="@/assets/image/Group.svg" alt="" />1205 руб.</a
            >
          </li>
          <li>
            <a href="/products" class="link-nav">
              <img src="@/assets/image/favorite.png" alt="" />Закладки</a
            >
          </li>
          <li>
            <a href="/contact" class="link-nav">
              <img src="@/assets/image/profile.svg" alt="" />Профиль</a
            >
          </li>
        </ul>
      </nav>
    </div>
    <div class="header-main">
      <div class="first-content">
        <img src="@/assets/image/logo-main.png" alt="" class="logo-main" />
        <div class="title-header-content">
          <h1 class="title-header">
            <span class="header-span">
              Stan Smith
            </span>,
          </h1>
          <div class="container-btn">
            <h1 class="title-header">
              Forever!
            </h1>
            <button class="btn btn-primary">Купить</button>
          </div>
        </div>
      </div>
      <img src="@/assets/image/header-main.png" alt="" />
    </div>
  </header>
</template>

<script>
import '@/assets/css/header.css'
export default {
  name: 'AppHeader'
}
</script>

<style scoped>
</style>
