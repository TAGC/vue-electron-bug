<template>
  <div>{{ message }}</div>
</template>

<script lang="js">
import Vue from "vue";

export default Vue.extend({
  props: {
    message: String
  }
})
</script>