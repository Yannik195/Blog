<template>
  <div id="app">
    <Header class="header"/>
    <BlogPost class="blogpost"
    v-for="post in posts"
    v-bind:key="post.id"
    v-bind:post="post"/>

    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import BlogPost from "./components/BlogPost.vue"
import Header from "./components/Header.vue"

export default {
  name: 'app',
  components: {
    HelloWorld,
    BlogPost,
    Header
  },
  data() {
    return {
          msg: "datamsg",
          posts: [
            {
              id: 1,
              date: "27. September",
              title: "Post One",
              text: "quia et suscipit suscipit recusandae consequuntur expedita et cum reprehenderit molestiae ut ut quas totam nostrum rerum est autem sunt rem eveniet architecto"
            },
            {
              id: 2,
              date: "11. Oktober",
              title: "Post Two",
              text: "est rerum tempore vitae sequi sint nihil reprehenderit dolor beatae ea dolores neque fugiat blanditiis voluptate porro vel nihil molestiae ut reiciendis qui aperiam non debitis possimus qui neque nisi nulla"
            }
          ]

    }
  }
}
</script>

<style>

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  max-width: 50rem;
  margin: 0 auto;
}


.blogpost{
  padding: 0 12px;

}


</style>
