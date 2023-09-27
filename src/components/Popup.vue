<script setup>
const props = defineProps(['subtitle', 'text', 'image']);
</script>

<template>
	<div class="popup">
		<div class="popup__image">
			<img
				:src="props.image"
				alt="Pizza">
		</div>
		<div class="popup__content">
			<h3>{{ props.subtitle }}</h3>
			<p>{{ props.text }}</p>
			<slot name="bottom"></slot>
		</div>
	</div>
</template>


<style scoped>
.popup {
  display: flex;
  flex-direction: row;
  align-items: flex-start;
  justify-content: flex-start;

  width: 480px;
  max-width: 480px;

  background-color: white;
  color: black;

	margin: 20px;
  border-radius: 16px;
  padding: 20px;
}

.popup__image {
  width: 160px;
  max-width: 160px;

  background-color: gray;
}

.popup__content h3 {
    font-size: 18px;
    font-family:Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
  }


.popup__content p {
  font-size: 48px;
  font-family:Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
}

.popup__subscribe {
  display: flex;
  flex-direction: row;
  align-items: flex-start;
  justify-content: flex-start;
}
</style>
