<template>
  <div id="helloWorldDiv">
    <div v-for='devName in devNames' :key="devName.id">
      <dev-summary-box :devName='devName' ></dev-summary-box>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';
import DevSummaryBox from '@/components/DevSummaryBox.vue'; // @ is an alias to /src

@Component({
  components: {
    DevSummaryBox,
  },
})
export default class HelloWorld extends Vue {
  data() {
    return {
      devNames: ['Michael', 'Paul', 'Matt', 'Srikar']
    }
  }
}
</script>

<style lang="scss" scoped>
.box {
  min-height: 15em;
  margin-bottom: 5em !important;
}
</style>

