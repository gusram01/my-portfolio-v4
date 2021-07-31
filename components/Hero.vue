<template>
  <section>
    <div class="img-container">
      <img src="~assets/img/gus.jpg" alt="gus photo" />
    </div>

    <h1>Gus Ramírez</h1>
    <h2>Frontend Jr</h2>

    <div class="icons">
      <IconLink :href="'https://github.com/gusram01'" :icon="'github-icon'" />
      <IconLink
        :href="
          'https://www.linkedin.com/in/gustavo-cesar-ramirez/?locale=en_US'
        "
        :icon="'linkedin-icon'"
      />
    </div>
  </section>
</template>

<script lang="ts">
import Vue from "vue";

import IconLink from "./IconLink.vue";

export default Vue.extend({
  components: { IconLink }
});
</script>

<style lang="postcss" scoped>
section {
  display: flex;
  flex-direction: column;
  align-items: center;
  min-height: 300px;
  padding-top: 5vh;
}
.img-container {
  width: 175px;
  border-radius: 50%;
}
.img-container > img {
  max-width: 100%;
  object-fit: cover;
}
</style>
