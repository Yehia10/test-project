<template>
  <div class="main">
    <h1>{{ PageDesc }}</h1>
    <h4>
      Email:
      <a target="_blank" href="mailto:yehia.maher2001@gmail.com">Text Me</a>
    </h4>
    <h5>Phone: <a target="_blank" href="tel:+2001027577313">Call Me</a></h5>
  </div>
</template>

<script>
export default {
  data() {
    return {
      PageName: "Help",
      PageDesc: "This Our Help Page",
    };
  },
  name: "HelpView",
};
</script>

<style scoped>
a {
  text-decoration: none;
}
</style>
