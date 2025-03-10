<template>
  <div :class="[$colorMode.preference]">
    <topbar />

    wassuppp

    <p>
      <nuxt-link to="/secondpage">Go to the second page</nuxt-link>
    </p>

    <button @click="toggleColorMode">
      Switch to {{ $colorMode.preference === 'dark' ? 'Light' : 'Dark' }} Mode
    </button>

  </div>
</template>

<script>

export default {
  methods: {
    toggleColorMode() {
      this.$colorMode.preference =
        this.$colorMode.preference === "dark" ? "light" : "dark";
    },
  },
};

</script>

<style scoped>

.light {
  background-color: white;
  color: black;
}

.dark {
  background-color: black;
  color: white;
}

</style>
