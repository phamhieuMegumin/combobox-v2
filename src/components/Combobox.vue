<template>
  <div class="combobox-container" @focusout="closeOptions">
    <div class="combobox-field" @click="isShow = !isShow"></div>
    <div class="combobox-options" v-if="isShow">
      <div class="option"></div>
      <div class="option"></div>
      <div class="option"></div>
      <div class="option"></div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isShow: false,
    };
  },
  methods: {
    closeOptions() {
      this.isShow = false;
      console.log("focusout");
    },
  },
};
</script>

<style scoped>
.combobox-container {
  width: 300px;
  position: relative;
}
.combobox-field {
  width: 300px;
  height: 42px;
  border: 1px solid #000;
  border-radius: 5px;
  cursor: pointer;
}
.combobox-options {
  position: absolute;
  width: 100%;
  top: calc(100% + 3px);
  border: 1px solid #000;
  border-radius: 5px;
}
.option {
  cursor: pointer;
  height: 42px;
}
.option:hover {
  background: greenyellow;
}
</style>
