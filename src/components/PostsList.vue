<template>
  <div class="list">

      <post-item v-for="post in posts" :key="post.id" v-bind:post="post"/>
     
  </div>
</template>

<script>
import axios from 'axios';
import PostItem from './PostItem';

export default {
  name: 'PostList',
  components: {
      PostItem
  },
  data () {
    return {
      posts: []
    }
  },

  mounted () {
      axios
      .get('https://jsonplaceholder.typicode.com/posts')
      .then(response => {
          console.log(response.data);

          this.posts = response.data
      })
  
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>