<template>
  <div class="post-box">
    <span class="post-views">1000</span>
    <h1 class="post-title">{{ upperCase(title) }} -N:{{ number }}</h1>
    <span class="post-date">21-10-2001</span>
    <p class="post-content">{{ content }}</p>
    <div class="row">
      <div class="col-sm-6">
        <p class="post-author">post author</p>
      </div>
      <div class="col-sm-6">
        <p class="post-category">post category</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["title", "content", "number"],
  name: "BlogPosts",
  methods: {
    upperCase(v) {
      return v.toUpperCase();
    },
  },
};
</script>

<style lang="scss" scoped>
.post-box {
  background-color: #fff;
  padding: 20px;
  position: relative;
  border-radius: 10px;
  box-shadow: 0 0 10px #9e9e9e;
  text-align: left;
  margin-bottom: 20px;
  margin-top: 20px;
  .post-views {
    position: absolute;
    top: 5px;
    right: 10px;
    background-color: #9e9e9e;
    padding: 2px 5px;
    color: white;
    font-weight: bold;
  }
  .post-content {
    padding: 10px 0px;
  }
  .post-category {
    text-align: right;
  }
}
</style>
