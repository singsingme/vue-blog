<template>
  <div class="modal_wrap">
    <div class="modal_content">
      <div>내용</div>
      <div @click="modalOpen()"><span class="material-symbols-outlined">close</span></div>
    </div>
  </div>
</template>

<script setup>
import { reactive, ref } from "vue";

// const emit = defineEmits(['modalCheck']);
// const modalCheck = ref(props.modalCheck)

let modalCheck = ref(false);

  function modalOpen() {
    modalCheck.value = !modalCheck.value
  }

</script>

<style lang="less">

</style>