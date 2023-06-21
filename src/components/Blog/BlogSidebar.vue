<template>
  <div class="side-bar">
    <h1>{{ pageDesc }}</h1>
    <p>Our Authors</p>
    <ol class="links">
      <li><a href="#">Author1</a></li>
      <li><a href="#">Author2</a></li>
      <li><a href="#">Author3</a></li>
      <li><a href="#">Author4</a></li>
    </ol>
  </div>
</template>

<script>
export default {
  name: "BlogSidebar",
  data() {
    return {
      pageDesc: "Side Bar Menu",
    };
  },
};
</script>

<style lang="scss" scoped>
.links {
  display: inline-block;
  li {
    a {
      text-decoration: none;
    }
  }
}
</style>
