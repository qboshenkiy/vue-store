<template>
  <main>
    <section id="search">
      <div class="container-search">
        <select class="filter">
          <option value="">Все кроссовки</option>
          <option value="">Jordan</option>
          <option value="">Nike</option>
        </select>
        <div class="search-container">
          <img src="@/assets/image/search.svg" alt="" />
          <input type="text" placeholder="Поиск..." class="search-input" />
        </div>
      </div>
    </section>

    <section id="product">
      <div class="container-product">
        <div class="product-item" v-for="(product, index) in products" :key="index">
          <img
            src="@/assets/image/favorite.png"
            alt=""
            class="favorite-icon"
            v-if="!product.isFavorite"
            @click="product.isFavorite = true"
          />
          <img
            src="@/assets/image/added_favorite.svg"
            alt=""
            class="favorite-icon"
            v-else
            @click="product.isFavorite = false"
          />

          <img :src="product.image" alt="" class="img-product" />
          <h3 class="product-title">{{ product.title }}</h3>

          <div class="container-price-product">
            <p class="product-price">
              <span class="price-span">Цена:</span><br />
              <strong>{{ product.price }} руб.</strong>
            </p>

            <button class="btn-buy" v-if="!product.isInCart" @click="product.isInCart = true">+</button>
            <img
              src="@/assets/image/added.svg"
              alt=""
              class="cart-icon"
              v-else
              @click="product.isInCart = false"
            />
          </div>
        </div>
      </div>
    </section>
  </main>
</template>

<script>
import '@/assets/css/main.css'
export default {
  name: 'AppMain',
  data () {
    return {
      products: [
        {
          title: 'Мужские Кроссовки Nike Air Max 270',
          price: 12000,
          image: require('@/assets/image/product/1.jpg'),
          isFavorite: false,
          isInCart: false
        },
        {
          title: 'Женские Кроссовки Adidas Yeezy Boost',
          price: 15000,
          image: require('@/assets/image/product/2.jpg'),
          isFavorite: false,
          isInCart: false
        },
        {
          title: 'Мужские Кроссовки Puma RS-X',
          price: 9000,
          image: require('@/assets/image/product/3.jpg'),
          isFavorite: false,
          isInCart: false
        },
        {
          title: 'Женские Кроссовки Reebok Classic',
          price: 8000,
          image: require('@/assets/image/product/4.jpg'),
          isFavorite: false,
          isInCart: false
        },
        {
          title: 'Мужские Кроссовки New Balance 574',
          price: 11000,
          image: require('@/assets/image/product/5.jpg'),
          isFavorite: false,
          isInCart: false
        },
        {
          title: 'Женские Кроссовки Nike Air Max 270',
          price: 13000,
          image: require('@/assets/image/product/6.jpg'),
          isFavorite: false,
          isInCart: false
        },
        {
          title: 'Мужские Кроссовки Adidas Ultraboost',
          price: 16000,
          image: require('@/assets/image/product/7.jpg'),
          isFavorite: false,
          isInCart: false
        },
        {
          title: 'Женские Кроссовки Asics Gel-Kayano',
          price: 14000,
          image: require('@/assets/image/product/8.jpg'),
          isFavorite: false,
          isInCart: false
        },
        {
          title: 'Мужские Кроссовки Saucony Jazz',
          price: 9500,
          image: require('@/assets/image/product/9.jpg'),
          isFavorite: false,
          isInCart: false
        },
        {
          title: 'Женские Кроссовки Hoka One One Bondi',
          price: 15500,
          image: require('@/assets/image/product/10.png'),
          isFavorite: false,
          isInCart: false
        }

      ]
    }
  }
}
</script>

<style></style>
