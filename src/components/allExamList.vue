<template>
  <div>
    <div class="col-12">
      <q-input
        label="Search for exams here"
        style="width: 70%"
        outlined
        rounded
      />
    </div>

    <div class="col-12">
      <div class="row q-ma-lg q-pt-sm flex items-center">
        <exam-card />
        <exam-card />
        <exam-card />
        <exam-card />
      </div>
    </div>
  </div>
</template>

<script>
import { defineComponent } from "vue";
import ExamCard from "./cards/ExamCard.vue";

export default defineComponent({
  components: { ExamCard },
  name: "examList",
});
</script>
<style scoped>
#exam-container {
  display: flex;
  flex-wrap: wrap;
  gap: 10px; /* Adjust this value to control the gap between items */
}

.col-5 {
  width: calc(10% - 10px); /* 10% width for each item with gap */
  margin-right: 20px; /* Adjust this value to control the gap between items */
}
</style>
