<template>
  <GeneralLayout>
    <Hero />
  </GeneralLayout>
</template>

<script lang="ts">
import Vue from "vue";

import GeneralLayout from "../layout/GeneralLayout.vue";
import Hero from "../components/Hero.vue";

export default Vue.extend({
  components: { GeneralLayout, Hero }
});
</script>
