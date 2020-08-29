<template>
  <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
    <div v-for="blog in placeholder_data" :key="blog.id">
      <BlogPost :data="blog" class=""/>
    </div>
  </div>
</template>

<script>
import BlogPost from '../ui/BlogPost';

export default {
  name: 'BlogPosts',
  data(){
    return {
      placeholder_data: [
        {
          id: 0,
          thumbnail: 'http://i3.ytimg.com/vi/q5J5ho7YUhA/maxresdefault.jpg',
          title: "Let's Build A Cool Button Animation",
          description: "We gonna build something cool today",
          content: "This is the content of the post"
        },
        {
          id: 1,
          thumbnail: 'http://i3.ytimg.com/vi/JjXBrJfp5TE/maxresdefault.jpg',
          title: "Project Managment Using Trello",
          description: "We gonna use Trello to do some managment",
          content: "This is the content of the post"
        },
        {
          id: 2,
          thumbnail: 'http://i3.ytimg.com/vi/gAkwW2tuIqE/maxresdefault.jpg',
          title: "Real-time Chat App Using Vue.js",
          description: "Let's build a chat app using Vue.js",
          content: "This is the content of the post"
        },
        {
          id: 3,
          thumbnail: 'http://i3.ytimg.com/vi/gAkwW2tuIqE/maxresdefault.jpg',
          title: "Real-time Chat App Using Vue.js",
          description: "Let's build a chat app using Vue.js",
          content: "This is the content of the post"
        }
      ]
    }
  },
  components: {
    BlogPost
  }
}
</script>

<style>

</style>