<template>
    <div>
        <button @click="toggleDarkMode">
            Toggle Dark Mode
        </button>
    </div>
</template>

<script setup>
const colorMode = useColorMode();

function toggleDarkMode() {
    colorMode.preference = colorMode.preference === "dark" ? "light" : "dark";
}
</script>

<style>
body {
    transition: background-color 0.3s, color 0.3s;
}

.dark-mode body {
    background-color: #121212;
    color: #ffffff;
}

.light-mode body {
    background-color: #ffffff;
    color: #000000;
}
</style>