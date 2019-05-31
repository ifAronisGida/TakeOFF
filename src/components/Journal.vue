<template>
  <div>
    <b-form-textarea
      id="textarea-rows"
      v-model="posts[0].content"
      @input="save"
      rows="10"
    ></b-form-textarea>
  </div>
</template>

<script>
import PostService from '@/api-services/post.service';

export default {
  name: 'Journal',
  data() {
    return {
      posts: [{ content: 'ez egy naplóbejegyzés' }],
    };
  },
  created() {
    PostService.getAll().then((response) => {
      this.posts = response.data;
    });
  },
  methods: {
    save(id) {
      PostService.update(this.posts[id].id, this.posts[id]);
    },
  },
};
</script>

<style scoped>

</style>
