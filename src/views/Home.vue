<template>
  <div class="home">
    <section class="container">
      <HelloWorld msg="Welcome to Your Vue.js + TypeScript App"/>
    </section>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import HelloWorld from '@/components/HelloWorld.vue'; // @ is an alias to /src

@Component({
  components: {
    HelloWorld,
  },
})
export default class Home extends Vue {}
</script>
