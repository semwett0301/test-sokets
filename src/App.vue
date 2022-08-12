<template>
  <div id="app">
    <Component1 :boot="c"/>
    <Component2 :boot="b"/>
  </div>
</template>

<script>

import Component1 from "@/components/Component1";
import Component2 from "@/components/Component2";
import uutil from "@/uutil";
export default {
  name: 'App',
  components: {
    Component1,
    Component2
  },
  data() {
    return {
      a: uutil.a,
      b: uutil.a,
      c: "fsadsf"
    }
  },
  updated() {
    console.log("Update main")
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
