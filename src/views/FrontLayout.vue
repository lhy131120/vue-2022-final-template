<template>
  <header>
    <nav class="navbar navbar-expand bg-light">
        <div class="container-fluid">
          <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav">
              <li class="nav-item"><router-link class="nav-link" to="/">Home</router-link></li>
              <li class="nav-item"><router-link class="nav-link" to="/products">貨品總覽</router-link></li>
              <li class="nav-item"><router-link class="nav-link" to="/news">最新消息</router-link></li>
              <li class="nav-item"><router-link class="nav-link" to="/about">關於我們</router-link></li>
              <li class="nav-item"><router-link class="nav-link" to="/rules">條款及細則</router-link></li>
              <li class="nav-item"><router-link class="nav-link" to="/qna">常見問題</router-link></li>
              <li class="nav-item"><router-link class="nav-link" to="/admin">登入</router-link></li>
            </ul>
          </div>
        </div>
      </nav>
  </header>
  <main>
    <router-view />
  </main>
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
