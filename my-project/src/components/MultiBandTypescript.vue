<!--<template>-->
<!--  <section v-for="(section, index) in responseData" :key="index">-->
<!--    <h1>{{ section.title || '' }}</h1>-->
<!--    <ul>-->
<!--      <li v-for="item in data" :key="item.id">{{ item.name }}</li>-->
<!--    </ul>-->
<!--  </section>-->
<!--</template>-->

<!--<script setup lang="ts">-->
<!--import axios from "axios";-->
<!--import { ref, onMounted } from "vue";-->

<!--const props = defineProps({-->
<!--  item: {-->
<!--    default: () => ({}),-->
<!--    type: Object-->
<!--  },-->
<!--});-->

<!--const data = ref([-->
<!--  { id: 1, name: '1' },-->
<!--  { id: 2, name: '2' },-->
<!--  { id: 3, name: '3' },-->
<!--  { id: 4, name: '4' },-->
<!--  { id: 5, name: '5' },-->
<!--]);-->
<!--const responseData = ref(null);-->

<!--onMounted(() => {-->
<!--  axios-->
<!--      .get('')-->
<!--      .then((response) => {-->
<!--        responseData.value = response.data.multisectionlist;-->
<!--        console.log(response.data);-->
<!--      })-->
<!--      .catch((error) => {-->
<!--        console.error('API 요청 중 오류 발생:', error);-->
<!--      });-->
<!--});-->
<!--</script>-->

<!--<style scoped>-->
<!--h1 {-->
<!--  margin: 0;-->
<!--  padding: 10px 10px;-->
<!--  color: white;-->
<!--}-->
<!--ul {-->
<!--  list-style-type: none;-->
<!--  padding: 0;-->
<!--  margin: 0;-->
<!--  overflow-y: scroll;-->
<!--  white-space: nowrap;-->
<!--}-->
<!--li {-->
<!--  display: inline-block;-->
<!--  margin: 10px 0 10px 10px;-->
<!--  padding: 40px 60px;-->
<!--  font-size: 30px;-->
<!--  color: white;-->
<!--  background-color: #282727;-->
<!--}-->
<!--</style>-->
