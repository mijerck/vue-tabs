<template lang="html">
  <div class="wrapper">
    <tabs>
      <tab title="Tab 1">
        Hello from Tab one
      </tab>
      <tab title="Tab 2">Hello From Tab 2</tab>
      <tab title="Tab 3">Hello From Tab 3</tab>
      <tab title="Tab 4">Hello From Tab 4</tab>
    </tabs>
  </div>
</template>

<script>
import Tab from "./Tab.vue";
import Tabs from "./Tabs.vue";

export default {
  data() {
    return {
      step: 0
    };
  },
  components: {
    Tab,
    Tabs
  },
  methods: {
    changeStyle() {
      console.log("change");
    }
  }
};
</script>

<style lang="css">
* {
  margin: 0;
  padding: 0;
  font-family: "Karla", sans-serif;
}
.wrapper {
  width: 100%;
  min-height: 100vh;
  background-color: #f8f8f8;
  margin: 0;
}

.change__style {
  background-color: #eee;
  font-size: 1em;
  margin-bottom: 10px;
  padding: 5px;
}
</style>
