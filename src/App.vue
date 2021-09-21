<template>
  <System v-if="loggedIn"/>
  <Auth v-else/>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import Auth from '@/views/Auth.vue';
import System from '@/views/System.vue';

export default defineComponent({
  name: 'App',
  data() {
    return {
      loggedIn: false,
    };
  },
  components: {
    Auth,
    System,
  },
  mounted() {
    if (localStorage.getItem('token')) {
      this.loggedIn = true;
    }
  },
});
</script>

<style>
#app {}
</style>
