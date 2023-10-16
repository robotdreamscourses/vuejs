<script setup>
import PopupComponent from "@/components/Popup.vue";
import SubscribeComponent from "@/components/Subscribe.vue";
import ButtonComponent from "@/components/Button.vue";
import ListingComponent from "@/components/Listing.vue";

const subtitle = "Limited Time Offer ⚠️"
const popimage = "https://images.unsplash.com/photo-1593560708920-61dd98c46a4e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=160&q=80"

</script>

<template>

	<ListingComponent></ListingComponent>

	<br>
	<hr>
	<br>
  <PopupComponent :subtitle="subtitle" text="Register and get 25% off on your next order!"
  :image="popimage">
  <template #bottom>
    <SubscribeComponent></SubscribeComponent>
  </template>
  </PopupComponent>

  <PopupComponent subtitle="Yeni bir popup 🦖" text="Begendiniz mi bu popup i?" :image="popimage">
  <template #bottom>
    <ButtonComponent text="Evet"></ButtonComponent>
    <ButtonComponent text="Hayir"></ButtonComponent>
  </template>
  </PopupComponent>

  <PopupComponent subtitle="Yeni bir popup 🦖" text="Begendiniz mi bu popup i?" :image="popimage"></PopupComponent>
</template>
