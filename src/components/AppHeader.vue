<template>
  <div class="header">
    <div class="container">
      <div class="logo">Yehya</div>
      <ul class="links text-end">
        <li><router-link to="/">Home</router-link></li>
        <li><router-link to="/about"> About</router-link></li>
        <li><router-link to="/help"> Help </router-link></li>
        <li><router-link to="/blog"> Blog </router-link></li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppHeader",
};
</script>

<style lang="scss" scoped>
.header {
  background-color: #333;
  padding: 20px;
  .container {
    display: flex;
    align-items: center;
  }
  .logo {
    color: #fff;
    font-size: 30px;
    width: 200px;
  }
  .links {
    width: calc(100% - 200px);
    li {
      display: inline-block;
      a {
        font-weight: bold;
        color: #fff;
        padding: 10px;
        text-decoration: none;
        font-size: 20px;
        &.router-link-exact-active {
          color: #42b983;
        }
      }
    }
  }
}
</style>
