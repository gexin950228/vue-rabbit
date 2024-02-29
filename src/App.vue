<script  setup>
import { getCategory } from './apis/testAPI'
getCategory().then(res => {
  console.log(res)
})

</script>

<template>
  <!-- 以及路由接口 -->
  <RouterView />
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}
.logo {
  display: block;
  margin: 0 auto 2rem;
}
nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}
</style>
