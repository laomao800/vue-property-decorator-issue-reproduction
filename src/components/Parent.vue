<template>
  <div class="hello">
    <Child/>
    <Child/>
  </div>
</template>

<script lang="ts">
import { Component, Vue, ProvideReactive } from "vue-property-decorator";
import Child from "./Child.vue";

@Component({
  components: {
    Child
  }
})
export default class Parent extends Vue {
  @ProvideReactive() formModel = {
    text1: "text1",
    text2: "text2"
  };
}
</script>
