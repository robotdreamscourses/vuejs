<script setup>
const props = defineProps(["title", "emoji"])
</script>

<template>
    <a href="#">
        <span>{{ props.emoji }}</span>
        {{ props.title }}
        <slot name="optional"></slot>
    </a>
</template>

<style scoped>
a {
    margin: 0 20px;
    padding: 8px 20px;
    background-color: blueviolet;
}
</style>