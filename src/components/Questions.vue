<template>
  <div class="container-fluid">
    <div class="row m-2 p-2"
         v-for="question in questions"
         :key="question.text">
      {{question.text}}</div>
  </div>
</template>

<script>
export default {
  name: 'Questions',
  data() {
    return {
      questions: [{ text: 'Mikor feküdtem le aludni?' },
        { text: 'Hány liter vizet ittam?' },
        { text: 'Hány órát tanultam?' }],
    };
  } };
</script>

<style scoped>

</style>
