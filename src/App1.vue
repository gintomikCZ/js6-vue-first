<template>
  <h1>js6 - first vue app</h1>
  <div>{{ `${label1} ${label2}` }}</div>
  <t-button :label="label1" />
  <!-- label má být 'click me' -->
  <p>
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Aliquam debitis iusto totam tempore ea
    vero itaque excepturi hic labore eos neque quaerat sit nihil, animi voluptatem consectetur
    voluptates? Facere, vero?
  </p>
  <t-button :label="label2" />
  <!-- label má být 'submit' -->

  <!-- v-bind: directive - shortcut ':'-->
  <TButton label="cokoliv" />

  <TButton :label="90"/>

</template>

<script>
import TButton from '@/components/TButton.vue'
// exportovat konfigurační objekt komponenty
export default {
  name: 'App',
  data() {
    return {
      label1: 'hdsufihsudfis',
      label2: 'rtzutuewrtewzu'
    }
  },
  components: { TButton }
}
</script>

<style>
h1 {
  color: red;
}
</style>
