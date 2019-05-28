<template>
  <div class="container-fluid d-flex h-100 flex-column" id="home_container">
    <div class="row d-flex flex-fill align-items-start">
      <div class="col-sm-8"><journal/></div>
      <div class="col-sm-4"><commitment class="justify-content-center"/></div>
    </div>
    <div class="row d-flex flex-fill align-items-center">
      <div class="col-sm-3"><questions/></div>
      <div class="col-sm-9"><answers/></div>
    </div>
    <div class="row flex-fill d-flex">
      <div class="col align-self-end">peer</div>
    </div>
  </div>
</template>
<script>
import Questions from '@/components/Questions';
import Journal from '@/components/Journal';
import Answers from '@/components/Answers';
import Commitment from '@/components/Commitment';

export default {
  name: 'Home',
  components: {
    Journal,
    Questions,
    Answers,
    Commitment,
  },
};
</script>
<style scoped>
  #home_container {
    min-height: 90vh;
  }
</style>
