<template>
  <h1>header</h1>
  <TList :listItems="fruits" />

  <div>
    <TInput label="first name" myId="first" :isDisabled="false" />
    <TInput label="last name" myId="last" :isDisabled="false" />
    <TInput label="your age" myId="age" inputType="number" :isDisabled="true" />
  </div>
</template>

<script>

import TList from '@/components/TList.vue'
import TInput from '@/components/TInput.vue'

export default {
  name: 'App',
  // data - musí to být funkce/metoda, která vrací objekt
  data: () => {
    return {
      fruits: ['banán', 'kiwi', 'hruška']
    }
  },
  components: { TList, TInput }
}



</script>