<template>
  <div id="About">
    <h1>This is an about page</h1>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator';

@Component({
  name: 'About'
})
export default class About extends Vue {}
</script>
