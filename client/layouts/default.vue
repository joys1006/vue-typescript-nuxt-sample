<template>
  <a-layout id="App">
    <app-aside />
    <a-layout id="container">
      <app-header />
      <a-layout-content id="content">
        <keep-alive>
          <nuxt />
        </keep-alive>
      </a-layout-content>
      <app-footer />
    </a-layout>
  </a-layout>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator';
import AppHeader from '@/components/Layouts/AppHeader/AppHeader.vue';
import AppFooter from '@/components/Layouts/AppFooter/AppFooter.vue';
import AppAside from '@/components/Layouts/AppAside/AppAside.vue';

@Component({
  name: 'Default',
  components: {
    AppHeader,
    AppFooter,
    AppAside
  }
})
export default class Default extends Vue {}
</script>

