<template>
  <div class="about">
    <h1 v-fontsize="60">About Me</h1>
    <div class="info-box">
      <div class="image">
        <img src="../assets/me.jpg" alt="Yehya Photo" />
      </div>
      <div class="info">
        <p v-fontsize="20">Name: Yehya Salem</p>
        <p v-fontsize="20">Age: 21</p>
        <p v-fontsize="20">Location: Mansoura</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AboutView",
  directives: {
    fontsize: {
      created: (el, binding) => (el.style.fontSize = binding.value + "px"),
    },
  },
};
</script>

<style lang="scss" scoped>
.info-box {
  display: flex;
  .image {
    width: 50%;
    img {
      max-width: 50%;
    }
  }
  .info {
    width: 50%;
    text-align: left;
  }
}
</style>
