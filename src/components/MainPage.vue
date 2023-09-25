<template>
  <div>
    <button @click="showPopup = true">Show modal</button>
    <SubPage v-show="showPopup" @close="closePopup" />
  </div>
</template>

<script>
import SubPage from "./SubPage.vue";
export default {
  name: "MainPage",
  components: { SubPage },
  data() {
    return { showPopup: false };
  },
  methods: {
    closePopup(name) {
      (this.showPopup = false), console.log("name", name);
    },
  },
};
</script>

<style scoped></style>
