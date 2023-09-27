<script setup>
const props = defineProps(['text']);

</script>
<template>
    <button>{{ props.text }}</button>
</template>

<style scoped>
button {
    border-radius: 12px;
    padding: 8px 14px;
    margin: 0 12px;
    background-color: bisque;
    font-size: 32px;
}
</style>