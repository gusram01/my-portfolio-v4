<template>
  <a class="link icon social" :href="href" target="_blank" rel="noreferrer">
    <span class="icon myicon" :class="icon" :aria-label="icon"></span>
  </a>
</template>
<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "IconLink",
  props: {
    href: {
      type: String,
      required: true
    },
    icon: {
      type: String,
      required: true
    }
  }
});
</script>
