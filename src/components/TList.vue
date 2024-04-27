<template>
  <ul>
    <li>{{ listItems[0] }}</li>
    <li>{{ listItems[1] }}</li>
    <li>{{ listItems[2] }}</li>
  </ul>
</template>

<script>
  export default {
    name: 'TList',
    props: {
      listItems: Array
    }
  }
</script>

<style scoped>
  ul {
    list-style-type: none;
  }
</style>