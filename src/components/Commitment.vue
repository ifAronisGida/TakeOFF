<template>
  <div class="container-fluid">
    <div class="row m-2 p-2 align-items-center"
         v-for="commitment in commitments"
         :key="commitment.id">
      <div v-if="commitment.goalType === 0" class="col align-content-center">
        {{ commitment.content }}
      </div>
    </div>
  </div>
</template>

<script>
import GoalsService from '@/api-services/goals.service';

export default {
  name: 'Commitment',
  data() {
    return {
      commitments: [],
    };
  },
  created() {
    GoalsService.getAll().then((response) => {
      this.commitments = response.data;
    });
  },
};
</script>

<style scoped>

</style>
