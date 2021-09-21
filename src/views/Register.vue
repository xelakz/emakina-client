<template>
  <Register/>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { useStore } from 'vuex';
import Register from '@/components/Register.vue';

export default defineComponent({
  name: 'Register View',
  data() {
    return {};
  },
  components: {
    Register,
  },
});
</script>
