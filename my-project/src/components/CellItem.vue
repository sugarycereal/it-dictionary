<template>
<!--  <li v-for="item in data" :key="item.id">{{ item.name }}</li>-->
</template>

<script>
import { ref } from "vue";

export default {
  name: 'CellList',
  setup(){
    const data = ref([
      { id: 1, name: '1' },
      { id: 2, name: '2' },
      { id: 3, name: '3' },
      { id: 4, name: '4' },
      { id: 5, name: '5' },
    ]);
    return {
      data,
    }
  },

}

</script>