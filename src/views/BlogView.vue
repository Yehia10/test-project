<template>
  <div class="main">
    <div class="container">
      <div class="row">
        <div class="col-md-8">
          <BlogPosts
            v-for="post in posts"
            :key="post.id"
            :title="post.title"
            :content="post.body"
            :number="post.id"
          />
        </div>
        <div class="col-md-4">
          <BlogSidebar />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import BlogPosts from "@/components/Blog/BlogPosts.vue";
import BlogSidebar from "@/components/Blog/BlogSidebar.vue";
import JsonPosts from "../json/posts.json";

export default {
  data() {
    return {
      PageName: "Blog",
      PageDesc: "This Our Blog Page",
      posts: JsonPosts,
    };
  },
  name: "BlogView",
  components: {
    BlogPosts,
    BlogSidebar,
  },
};
</script>
