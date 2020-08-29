<template>
  <div>
    <AppHero>
      <div
        class="hero-content flex flex-col items-start justify-start text-white text-xl md:text-2xl pt-20 px-1 md:pt-0 md:pb-20 md:justify-center md:px-20"
      >
        <h1>
          Welcom to <span class="logo-font red">{Bushido Code}</span>
        </h1>
        <h1>
          Where, with the ways of the
          <span class="logo-font red">Samurai</span>
        </h1>
        <h1>
          we forge our
          <span class="logo-font red">Code</span>
        </h1>
      </div>
    </AppHero>
    
    <div class="homepage-content px-10 py-10">
      <BlogPosts/>
    </div>
  </div>
</template>

<script>
import AppHero from "../components/layout/AppHero";
import BlogPosts from "../components/layout/BlogPosts";

export default {
  name: "HomePage",
  components: {
    AppHero,
    BlogPosts
  }
};
</script>

<style scoped>
.hero-content {
  height: 100%;
  font-weight: bold;
}
</style>
