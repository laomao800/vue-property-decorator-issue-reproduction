<template>
  <div class="hello">
    <ChildExpect/>
    <ChildExpect/>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import ChildExpect from "./ChildExpect.vue";

@Component({
  provide() {
    return {
      reactive: {
        formModel: {
          text1: 1,
          text2: 2
        }
      }
    };
  },
  components: {
    ChildExpect
  }
})
export default class ParentExpect extends Vue {}
</script>
