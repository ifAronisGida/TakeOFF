<template>
  <div class="container-fluid">
    <div class="row align-items-start border border-info">
      <div class="col-sm-1 border border-info">tegnap</div>
      <div class="col-sm-8 border border-info"><journal/></div>
      <div class="col-sm-3 border border-info">vállalás</div>
    </div>
    <div class="row align-item-center border border-info">
      <div class="col-sm-3 border border-info"><questions/></div>
      <div class="col-sm-9 border border-info"><answers/></div>
    </div>
    <div class="row align-items-end border border-info">
      <div class="col border border-info">peer</div>
    </div>
  </div>
</template>
<script>
import OneDayTab from '@/components/OneDayTab';
import Questions from '@/components/Questions';
import Journal from '@/components/Journal';
import Answers from '@/components/Answers';

export default {
  name: 'Home',
  components: {
    'one-day': OneDayTab,
    Journal,
    Questions,
    Answers,
  },

  data() {
    return {
      posts: [
        { id: 1,
          date: '2019-05-10',
          text: [
            { id: 1, question: 'Question 1', answer: 'daily answer' },
            { id: 2, question: 'Q2', answer: 'daily asdlfkj séodifh aséldk fhaséd hfaosidh fanswer' },
            { id: 3, question: 'question 3', answer: 'daily answer' },
            { id: 4, question: 'question 4', answer: 'daily asdf' },
            { id: 5, question: 'question 5', answer: 'daiasdfasdfly answer' },
            { id: 6, question: 'question 5', answer: 'daiasdfasdfly answer' },
            { id: 7, question: 'question 5', answer: 'daiasdfasdfly answer' },
            { id: 8, question: 'question 5', answer: 'daiasdfasdfly answer' },
            { id: 9, question: 'question 5', answer: 'daiasdfasdfly answer' },
            { id: 10, question: 'question 5', answer: 'daiasdfasdfly answer' },
            { id: 101, question: 'question 5', answer: 'daiasdfasdfly answer' }] },
        { id: 2,
          date: '2019-05-11',
          text: [
            { id: 1, question: 'peerq1', answer: 'daily answer' },
            { id: 2, question: 'questionpeer2', answer: 'daily answer' },
            { id: 3, question: 'questionpee3', answer: 'asdf answer' },
            { id: 4, question: 'questionasdf', answer: 'daily answer' },
            { id: 5, question: 'questionsdf', answer: 'daily answer' }] },
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
