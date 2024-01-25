<template>
  <div id="content">
    <div class="content_box" @click="modalOpen()" v-for="(iteam, index) in iteams" :key="index">
      {{ iteam.title }}
      {{ iteam.badge }}
    </div>
    <PortfoiloModal v-show="modalCheck"/>
  </div>
</template>

<script setup>
import { reactive, ref } from "vue";
import PortfoiloModal from "./PortfoiloModal.vue"
  // const props = defineProps({
  //   modalCheck: Boolean
  // });

  let modalCheck = ref(false);

  let iteams = reactive([
    {imgSrc: '', title: '제목1', badge: 'vue'},
    {title: '제목2', badge: 'vue'},
    {title: '제목3', badge: 'vue'},
    {title: '제목4', badge: 'vue'},
    {title: '제목5', badge: 'vue'}
  ]);
  
  function modalOpen() {
    console.log(modalCheck)
    modalCheck.value = !modalCheck.value
  }

</script>

<style lang="less">
  #content {
    width: 100%;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    padding: 100px;
    position: relative;
    .content_box {
      width: 23%;
      height: 300px;
      // border: 1px solid black;
      border-radius: 20px;
      margin-bottom: 50px;
      box-shadow: 1px 1px 3px 1px #dadce0;
    }
  }
</style>