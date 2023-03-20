<template>
  <header>
    <nav class="navbar navbar-expand bg-primary">
        <div class="container">
          <div class="collapse navbar-collapse flex-wrap" id="navbarNav">
            <div class="d-flex justify-content-between align-items-center w-100">
              <router-link to="/home"><img src="/logo.png" style="width: 228px;" alt="Logo" class="logo"></router-link>
              <ul class="navbar-nav">
                <li class="nav-item me-9"><a class="nav-link nav-icon nav-cart" href="javascript:;">Cart</a></li>
                <!-- <li class="nav-item"><a class="nav-link nav-icon nav-login" href="javascript:;">Login</a></li> -->
                <li class="nav-item"><router-link class="nav-link nav-icon nav-login" to="/admin">登入</router-link></li>
              </ul>
            </div>
            <div class="w-100">
              <ul class="navbar-nav justify-content-center">
                <li class="nav-item"><router-link class="nav-link mx-5" to="/products">貨品總覽</router-link></li>
                <li class="nav-item"><router-link class="nav-link mx-5" to="/news">最新消息</router-link></li>
                <li class="nav-item"><router-link class="nav-link mx-5" to="/about">關於我們</router-link></li>
                <li class="nav-item"><router-link class="nav-link mx-5" to="/rules">條款及細則</router-link></li>
                <li class="nav-item"><router-link class="nav-link mx-5" to="/qna">常見問題</router-link></li>
              </ul>
            </div>
          </div>
        </div>
      </nav>
      <div class="bannerWrap">
        Banner
      </div>
  </header>
  <main>
    <router-view />
  </main>
  <footer class="footer bg-primary text-center">
    <div class="container">
      <div class="pt-6 pt-md-6 pb-7 pb-md-5">
        <img src="/logo.png" style="width: 228px;" alt="Logo" class="logo">
        <ul class="nav row row-cols-3 row-cols-lg-6 g-2 mt-5 mb-5 pb-4 border border-top-0 border-start-0 border-end-0">
          <li class="col nav-item m-0"><router-link class="nav-link p-2" to="/home">首頁</router-link></li>
          <li class="col nav-item m-0"><router-link class="nav-link p-2" to="/products">貨品總覽</router-link></li>
          <li class="col nav-item m-0"><router-link class="nav-link p-2" to="/news">最新消息</router-link></li>
          <li class="col nav-item m-0"><router-link class="nav-link p-2" to="/about">關於我們</router-link></li>
          <li class="col nav-item m-0"><router-link class="nav-link p-2" to="/rules">條款及細則</router-link></li>
          <li class="col nav-item m-0"><router-link class="nav-link p-2" to="/qna">常見問題</router-link></li>
        </ul>
        <p class="text-success mb-0">Copyright @2022 DeliFans All rights reserved.</p>
      </div>
    </div>
  </footer>
</template>

<script>
import { RouterView, RouterLink } from 'vue-router'
export default {
  components: {
    RouterView,
    RouterLink
  }
}
</script>
