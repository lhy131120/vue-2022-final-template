<template>
  <header>
    <nav class="navbar navbar-expand bg-light">
        <div class="container-fluid">
          <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav">
              <li class="nav-item"><router-link class="nav-link" to="/">Home</router-link></li>
              <li class="nav-item"><router-link class="nav-link" to="/admin/products">後台貨品列表</router-link></li>
              <li class="nav-item"><router-link class="nav-link" to="/admin/orders">後台訂單列表</router-link></li>
              <li class="nav-item"><router-link class="nav-link" to="/">登出</router-link></li>
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
const { VITE_URL, VITE_API } = import.meta.env


export default {
  components: {
    RouterView,
    RouterLink
  },
  mounted () {
    console.log(VITE_URL, VITE_API)
  }
}
</script>
