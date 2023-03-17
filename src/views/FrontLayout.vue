<template>
  <header>
    <nav class="navbar navbar-expand bg-primary">
        <div class="container">
          <div class="collapse navbar-collapse flex-wrap" id="navbarNav">
            <div class="d-flex justify-content-between">
              <router-link to="/"><img src="/logo.png" style="width: 228px;" alt="Logo" class="logo"></router-link>
              <ul class="navbar-nav">
                <li class="nav-item"><a class="nav-link nav-cart" href="javascript:;">Cart</a></li>
                <li class="nav-item"><a class="nav-link nav-login" href="javascript:;">Login</a></li>
              </ul>
            </div>
            <div class="w-100">
              <ul class="navbar-nav">
                <li class="nav-item"><router-link class="nav-link" to="/products">貨品總覽</router-link></li>
                <li class="nav-item"><router-link class="nav-link" to="/news">最新消息</router-link></li>
                <li class="nav-item"><router-link class="nav-link" to="/about">關於我們</router-link></li>
                <li class="nav-item"><router-link class="nav-link" to="/rules">條款及細則</router-link></li>
                <li class="nav-item"><router-link class="nav-link" to="/qna">常見問題</router-link></li>
                <li class="nav-item"><router-link class="nav-link" to="/admin">登入</router-link></li>
              </ul>
            </div>
          </div>
        </div>
      </nav>
  </header>
  <main>
    <router-view />
  </main>
  <footer class="bg-primary text-center">
    <div class="container">
      <div>
        <img src="/logo.png" style="width: 228px;" alt="Logo" class="logo">
      </div>
      <ul class="navbar-nav">
        <li class="nav-item"><router-link class="nav-link" to="/">首頁</router-link></li>
        <li class="nav-item"><router-link class="nav-link" to="/products">貨品總覽</router-link></li>
        <li class="nav-item"><router-link class="nav-link" to="/news">最新消息</router-link></li>
        <li class="nav-item"><router-link class="nav-link" to="/about">關於我們</router-link></li>
        <li class="nav-item"><router-link class="nav-link" to="/rules">條款及細則</router-link></li>
        <li class="nav-item"><router-link class="nav-link" to="/qna">常見問題</router-link></li>
      </ul>
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
