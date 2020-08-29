<template>
  <div class="shadow-xl relative">
    <img :src="data.thumbnail" class="thumbnail">
    <button class="btn article-btn">Read</button>
  </div>
</template>

<script>
export default {
  name: 'BlogPost',
  props: ['data']
}
</script>

<style scoped>
.article-btn{
  width: 100%;
}
.article-btn:hover{
  color: var(--white);
}
</style>