<template>
  <div style="display:flex;">
    <div style="border:1px solid #ddd;margin-right:30px;">
      <h2>Error Sample</h2>
      <h3>Parent 1</h3>
      <Parent />
      <h3>Parent 2</h3>
      <p>Change these values will effects 'parent 1'</p>
      <Parent />
    </div>

    <div style="border:1px solid #ddd;">
      <h2>Expect Sample</h2>
      <h3>Parent 1</h3>
      <ParentExpect />
      <h3>Parent 2</h3>
      <p>Expect use a new provide model in each 'Parent'</p>
      <ParentExpect />
    </div>
  </div>
</template>

<script>
import Parent from './components/Parent.vue'
import ParentExpect from './components/ParentExpect.vue'

export default {
  components: {
    Parent,
    ParentExpect
  }
}
</script>
