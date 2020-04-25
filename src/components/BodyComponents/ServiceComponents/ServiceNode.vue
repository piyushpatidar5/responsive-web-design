<template>
  <div class="ServiceNodeContainer">
    <div class="Icon_ServiceNameContainer">
      <i :class="'ServiceIcon fas '+nodeData.icon"></i>
      <span class="ServiceNameLabel">{{nodeData.name}}</span>
    </div>
  </div>
</template>


<script>
export default {
  name: "ServiceNode",
  components: {},
  props: ["nodeData"],
  data() {
    return {
      a: ""
    };
  }
};
</script>
