<template>
  <main :class="colorTheme">
    <header>
      <button class="button icon" @click="changeTheme">
        theme
      </button>
    </header>
    <slot></slot>
  </main>
</template>

<script lang="ts">
import Vue from "vue";
export default Vue.extend({
  data() {
    return {
      lightTheme: true
    };
  },

  computed: {
    colorTheme(): string {
      return this.lightTheme ? "light-theme" : "dark-theme";
    }
  },

  methods: {
    changeTheme() {
      this.lightTheme = !this.lightTheme;
    }
  }
});
</script>

<style lang="postcss" scoped>
main {
  position: relative;
  width: 100%;
  height: 100%;
  min-height: 100vh;
  max-width: 1366;
  margin: 0 auto;
}
header {
  position: sticky;
  padding-top: 2vh;
  padding-right: 2vh;
  text-align: right;
}
</style>
