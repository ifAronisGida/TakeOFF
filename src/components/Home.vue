<template>
  <div>
    <b-tabs content-class="mt-3" fill>
      <b-tab
        v-for="post in posts"
        :key="post.id"
        :title="post.date">
        <one-day :text="post.text"/>
      </b-tab>
    </b-tabs>
  </div>
</template>
<script>
import OneDayTab from '@/components/OneDayTab';

export default {
  name: 'Home',
  components: {
    'one-day': OneDayTab,
  },
  data() {
    return {
      posts: [
        { id: 1,
          date: '2019-05-10',
          text: [
            { id: 1, question: 'sdfasdfasdf question', answer: 'daily answer' },
            { id: 2, question: 'daily question', answer: 'daily asdlfkj séodifh aséldk fhaséd hfaosidh fanswer' },
            { id: 3, question: 'daily question', answer: 'daily answer' },
            { id: 4, question: 'daily question', answer: 'daily answer' },
            { id: 5, question: 'daily question', answer: 'daily answer' }] },
        { id: 2,
          date: '2019-05-11',
          text: [
            { id: 1, question: 'daily asdf', answer: 'daily answer' },
            { id: 2, question: 'daily question', answer: 'daily answer' },
            { id: 3, question: 'daily question', answer: 'daily answer' },
            { id: 4, question: 'daily question', answer: 'daily answer' },
            { id: 5, question: 'daily question', answer: 'daily answer' }] },
        { id: 3,
          date: '2019-05-12',
          text: [
            { id: 1, question: 'daily question', answer: 'daily answer' },
            { id: 2, question: 'daily question', answer: 'daily answer' },
            { id: 3, question: 'daily question', answer: 'dailyasdfasdf answer' },
            { id: 4, question: 'daily question', answer: 'daily answer' },
            { id: 5, question: 'daily question', answer: 'daily answer' }] },
        { id: 4,
          date: '2019-05-13',
          text: [
            { id: 1, question: 'daily question', answer: 'daily answer' },
            { id: 2, question: 'daily question', answer: 'daily answer' },
            { id: 3, question: 'dailyasdfasdf question', answer: 'daily answer' },
            { id: 4, question: 'daily question', answer: 'daily answer' },
            { id: 5, question: 'daily quasdfasdfestion', answer: 'daily answer' }] },
        { id: 5,
          date: '2019-05-14',
          text: [
            { id: 1, question: 'daily question', answer: 'daily answer' },
            { id: 2, question: 'dailasdfasdfy question', answer: 'daily answer' },
            { id: 3, question: 'daily question', answer: 'daily answer' },
            { id: 4, question: 'daily question', answer: 'daily answer' },
            { id: 5, question: 'daily question', answer: 'dailasdfasdfy answer' }] },
      ],
    };
  },
};
</script>
<style scoped>
</style>
