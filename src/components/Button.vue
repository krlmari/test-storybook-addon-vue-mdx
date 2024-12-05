<!-- eslint-disable vue/multi-word-component-names -->
<script setup>

defineProps({
  label: {
    type: String,
    required: true,
  },
});

const emit = defineEmits(['click']);

const onClick = () => {
  emit('click');
};
</script>

<template>
  <button 
    type="button" 
    @click="onClick" 
>
    {{ label }}
  </button>
</template>

<!-- 
<style scoped>
  button {
    display: inline-flex;
    justify-content: center;
    align-items: center;
    padding: 20px;
    border-radius: 1000px;
    border: none;
    background: #cacaca; 
    color: #313131;
    font-size: 16px;
    font-weight: bold;
    cursor: pointer;
  }
</style>
-->


