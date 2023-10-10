<template>
  <ul>
    <CellItem />
  </ul>
</template>

<script>
import { ref } from "vue";
import CellItem from "@/components/CellItem.vue";

export default {
  name: 'CellList',
  components: {CellItem},

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