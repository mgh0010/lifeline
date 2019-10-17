<template>
  <div id="dev-summary-box-div">
    <div class="box">{{devName}}</div>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class DevSummaryBox extends Vue {
  @Prop() private devName!: string;
}
</script>

<style lang="scss" scoped>
.box {
  min-height: 15em;
}
</style>