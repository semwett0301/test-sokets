<template>
<div>
  <input v-model="boot">
</div>
</template>

<script>
export default {
  name: "Component1",
  props: {
    boot: String
  },
  updated() {
    console.log("Update 1")
  }
}
</script>

<style scoped>

</style>
