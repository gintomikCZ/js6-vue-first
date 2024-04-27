<template>
  <button>{{ label }}</button>
</template>

<script>
/* interpolace - způsob jak přenést JS výraz do HTML template */

/*
props - properties
a) pole s názvy jednotlivých props
b) objekt {
  prop: datový typ
}
c) objekt {
  prop: {
    type: String,
    required: true
  }
}

!!!! nikdy nesmí měnit propsu
*/
export default {
  name: 'TButton',
  props: {
    label: String
  }
}
</script>

<style scoped>
button {
  background: white;
  border: 1px solid #454545;
  padding: 0.35em 0.7em;
  border-radius: 4px;
  font-size: 1rem;
  color: black;
  transition: background-color 0.4s ease;
}
button:hover {
  background: var(--button-hover-bg);
}
</style>
