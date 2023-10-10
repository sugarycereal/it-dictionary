<template>
  <section class="hello">
    <h1>{{ msg }}</h1>
    <ul>
      <li v-for="item in data" :key="item.id">{{ item.name }}</li>
    </ul>
  </section>
</template>

<script>
export default {
  name: 'MultiBand',
  props: {
    msg: String
  },
  setup(){
    const data = [
      { id: 1, name: '1' },
      { id: 2, name: '2' },
      { id: 3, name: '3' },
      { id: 4, name: '4' },
      { id: 5, name: '5' },
    ]
    return {data}
  }
}

</script>

<style scoped>
section {
  background-color: #4a5959;
}
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
