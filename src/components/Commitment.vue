<template>
  <div class="container-fluid">
    <div class="row m-2 p-2 align-items-center"
         v-for="commitment in commitments"
         :key="commitment.text">
      <div class="col align-content-center">
        {{ commitment.text }}
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Commitment',
  data() {
    return {
      commitments: [
        { text: 'felvesznek a microsofthoz' },
        { text: 'felvesznek a microsofthoz' },
        { text: 'felvesznek a microsofthoz' },
        { text: 'felvesznek a microsofthoz' },
        { text: 'felvesznek a microsofthoz' },
      ],
    };
  },
};
</script>

<style scoped>

</style>
