<template>
  <h1>{{ section.title || '' }}</h1>
</template>

<script>

export default {
  name: 'CellList',
  props: {
    title: String
  },

}

</script>