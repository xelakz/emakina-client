<template>
  <router-view/>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { useStore } from 'vuex';

export default defineComponent({
  name: 'System View',
  data() {
    return {
      route: '/login',
    };
  },
  props: {
    title: String,
  },
  mounted() {
    this.route = this.$route.path;
    console.log(this.$route.path);
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .auth {
    width: 300px;
  }

  .auth .btn-wrapper {
    text-align: right;
  }
</style>
