<template>
  <div class="home">
    <h1>{{ pageDesc }}</h1>
  </div>
</template>

<script>
export default {
  name: "HomeView",
  data() {
    return {
      pageDesc: "Welcome To Our Page",
    };
  },
};
</script>
