<template>
  <div>
    <b-tabs content-class="mt-3" fill>
      <b-tab
        v-for="post in posts"
        :key="post.id"
        :title="post.date">
        <p>{{ post.text }}</p>
      </b-tab>
    </b-tabs>
  </div>
</template>
<script>
export default {
  name: 'Home',
  data() {
    return {
      posts: [
        { id: 1, date: '2019-05-10', text: { question: 'daily question', answer: 'daily answer' } },
        { id: 2, date: '2019-05-11', text: { question: 'daily question', answer: 'daily answer' } },
        { id: 3, date: '2019-05-12', text: { question: 'daily question', answer: 'daily answer' } },
        { id: 4, date: '2019-05-13', text: { question: 'daily question', answer: 'daily answer' } },
        { id: 5, date: '2019-05-14', text: { question: 'daily question', answer: 'daily answer' } },
        { id: 6, date: '2019-05-15', text: { question: 'daily question', answer: 'daily answer' } },
      ],
    };
  },
};
</script>
<style scoped>
</style>
