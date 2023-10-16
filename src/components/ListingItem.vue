<script setup>
const props = defineProps(['emoji', 'name', 'lastname', 'experience']);
</script>

<template>
	<li  v-if="props.experience < 5" style="color: purple;">
		{{ props.name }} {{ props.lastname }} - {{ props.emoji }}
	</li>
	<li v-else>
		{{ props.name }}
	</li>
</template>
