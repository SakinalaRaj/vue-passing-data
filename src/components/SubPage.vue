<template>
  <div>
    <h3>This is Sub Page</h3>
    <button @click="$emit('close', 'raju')">Hide this Subpage</button>
  </div>
</template>

<script>
export default {
  name: "SubPage",
  emits: ["close"],
};
</script>

<style scoped></style>
