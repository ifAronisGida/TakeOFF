<template>
  <div class="container-fluid">
    <div class="m-2 p-2" v-for="answer in answers" :key="answer.answer">{{ answer.answer }}</div>
  </div>
</template>

<script>
export default {
  name: 'Answers',
  data() {
    return {
      answers: [
        { answer: 'Korán sikerült feküdnöm: 9pm' },
        { answer: 'csak 1 :(' },
        { answer: '5 !!!!' },
      ],
    };
  },
};
</script>

<style scoped>

</style>
