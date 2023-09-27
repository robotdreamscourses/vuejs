<script setup>
import MenuItem from "@/components/Menu/MenuItem.vue"

const menuFirstTitle = "Ana Sayfa 2";
const menuSecondTitle = "Iletisim 1"
</script>

<template>
    <nav>
        <MenuItem :title="menuFirstTitle" emoji="🦄"></MenuItem>
        <MenuItem :title="menuSecondTitle"></MenuItem>
        <MenuItem title="Yardim Sayfasi">
            <template #optional>
                🦖 <strong>Robot Dreams</strong>
                <p>Lorem ipsum dolor sit amet.</p>
                <button>Button</button>
            </template>
        </MenuItem>
    </nav>
</template>