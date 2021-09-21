<template>
  <Login/>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { useStore } from 'vuex';
import Login from '@/components/Login.vue';

export default defineComponent({
  name: 'Login View',
  data() {
    return {};
  },
  components: {
    Login,
  },
});
</script>
