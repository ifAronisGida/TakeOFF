<template>
  <div>
    <b-form-textarea
      id="textarea-rows"
      v-model="posts[6].content"
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
      posts: [],
    };
  },
  created() {
    PostService.getAll().then((response) => {
      this.posts = response.data;
    });
  },
  methods: {
    save() {
      PostService.update(this.posts[6].id, this.posts[6]);
    },
  },
};
</script>

<style scoped>

</style>
