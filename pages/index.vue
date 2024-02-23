<template>
  <div>
    <h1>
      Wait for 5 second to ref effect:
      <p v-html="text"></p>
    </h1>
    <p>Email comes using Reactive Property : {{ formData.email }}</p>
    <p>Use of Computed Property: {{ getResult }}</p>
    <button @click="count++" class="border-2 p-2">Increase Count</button>
    <p>{{ count }}</p>
    <button @click="count--" class="border-2 p-2">Decrease Count</button>
  </div>
</template>
<script setup>
import { ref, reactive, computed, watch } from "vue";

const text = ref("Ref Value");
const formData = reactive({
  firstName: "Vidhi",
  lastName: "Suthar",
  email: "vidhi@7span.com",
});
const dollors = 100;
const rupeeValue = 80;
const discount = 10;
const count = ref("0");

const getResult = computed(() => {
  return (dollors * rupeeValue) / discount;
});

watch(count, (newvalue, oldvalue) => {
  console.log("New Count is : ", newvalue, oldvalue);
});

setTimeout(() => {
  text.value = "<b>Update Ref Value</b>";
}, 5000);
</script>
