<template>
  <div>
    <input v-model="formModel.text1">
    <input v-model="formModel.text2">
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component({
  inject: ["reactive"]
})
export default class ChildExpect extends Vue {
  // @ts-ignore
  formModel = this.reactive.formModel;
}
</script>
