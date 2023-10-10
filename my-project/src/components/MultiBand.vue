<template>
  <section v-for="(section, index) in responseData" :key="index">

  </section>
</template>

<script>
import axios from "axios";
import { ref } from "vue";
// import CellList from "@/components/CellList.vue";
// import CellTitle from "@/components/CellTitle.vue";

export default {
  name: 'MultiBand',
  // components: {CellTitle,CellList},
  setup(){
    const responseData = ref(null);
    return {
      responseData
    }
  },

  beforeCreate() {
    axios.get('https://apis.wavve.com/v1/multiband/GN51?client=40&apikey=E5F3E0D30947AA5440556471321BB6D9&client_version=6.1.0&device=mobile&drm=wm&partner=pooq&pooqzone=none&region=kor&service=wavve&targetage=all')
    .then(response => {
      this.responseData = response.data.multisectionlist;
      console.log(response.data);
    })
    .catch(error => {
      console.error('API 요청 중 오류 발생:', error);
    });
  },

}

</script>

<style scoped>
h1 {
  margin: 0;
  padding: 10px 10px;
  color: white;
}
ul {
  list-style-type: none;
  padding: 0;
  margin: 0;
  overflow-y: scroll;
  white-space: nowrap;
}
li {
  display: inline-block;
  margin: 10px 0 10px 10px;
  padding: 40px 60px;
  font-size: 30px;
  color: white;
  background-color: #282727;
}
</style>
