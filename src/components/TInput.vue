<template>
  <div>
    <label :for="myId">{{ label }}</label>
    <input :id="myId" :type="inputType" :disabled="isDisabled"/>
  </div>
</template>

<script>
export default {
  props: {
    label: {
      type: String,
      required: true,
    },
    myId: {
      type: String,
      required: true
    },
    inputType: {
      type: String,
      default: 'text'
    },
    isDisabled: {
      type: Boolean
    }
  }
}
</script>
