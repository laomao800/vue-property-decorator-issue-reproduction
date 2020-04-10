<template>
  <div>
    <input v-model="formModel.text1">
    <input v-model="formModel.text2">
  </div>
</template>

<script lang="ts">
import { Component, Vue, InjectReactive } from "vue-property-decorator";

@Component
export default class Child extends Vue {
  @InjectReactive() formModel!: any;
}
</script>
