<template>
  <div>
    {{boot}}
  </div>
</template>

<script>
export default {
  name: "Component2",
  props: {
    boot: String
  },
  updated() {
    console.log("Update 2")
  }
}
</script>

<style scoped>

</style>
