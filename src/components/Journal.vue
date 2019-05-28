<template>
  <div>
    <b-form-textarea
      id="textarea-rows"
      :value="journalEntry.description"
      rows="10"
    ></b-form-textarea>
  </div>
</template>

<script>
import JournalService from '@/api-services/journal.service';

export default {
  name: 'Journal',
  data() {
    return {
      journalEntry: { description: "Mai nap rengeteg dolog történt velem például elmentem sétálni és láttam egy " +
          "kutyát meg egy virágot és vettem egy palackozott sört is" +
          "finomat főzőtt anyukám is" +
          "we like to type!!!4"},
    };
  },
};
</script>

<style scoped>

</style>
