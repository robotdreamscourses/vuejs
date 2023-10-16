<script setup>
import ListingItem from "@/components/ListingItem.vue"
const data = [
	{
		id: 1,
		name: "Tolga",
		lastname: "Egilmezel",
		emoji: "🍕",
		experience: 18
	},
	{
		id: 2,
		name: "Filiz",
		lastname: "Altinturk",
		emoji: "👻",
		experience: 16
	},
	{
		id: 3,
		name: "Robot Dreams",
		lastname: "Laba",
		emoji: "🐿️",
		experience: 2
	}
]
</script>

<template>
<div>
	<ul>
			<ListingItem v-for="person in data" :key="person.id" :name="person.name" :lastname="person.lastname" :emoji="person.emoji" :experience="person.experience"></ListingItem>
	</ul>
	<br>
	<hr>
	<br>
	<ul>
		<ListingItem v-for="person in data" :key="person.id" :name="person.name" :lastname="person.lastname" :emoji="person.emoji" :experience="person.experience"></ListingItem>
	</ul>
	<br>
	<ul>
		<li v-for="(person, index) in data">
			<ListingItem :name="person.name" :lastname="person.lastname" :emoji="person.emoji"></ListingItem>
		</li>
	</ul>
</div>
</template>
