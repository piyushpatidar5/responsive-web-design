<template>
  <div id="ServiceContainer" class="DisplayFlexBox">
    <div class="ServiceCards_HeadingContainer">
      <div class="HeadingContainer">
        <span class="ServiceHeading">Integer bibendum sit amet arcu vel egestas.</span>
      </div>
      <div class="ServiceCardsContainer">
        <div class="DesktopMobileNodes" :key="index" v-for="(node,index) in services">
          <ServiceNode :nodeData="node"/>
        </div>
      </div>
    </div>
  </div>
</template>


<script>
import ServiceNode from "./ServiceComponents/ServiceNode.vue";
export default {
  name: "ServiceContainer",
  components: {
    ServiceNode
  },
  data() {
    return {
      services: [
        {
          name: "Service Name 1",
          icon: "fa-users"
        },
        {
          name: "Service Name 2",
          icon: "fa-user-cog"
        },
        {
          name: "Service Name 3",
          icon: "fa-cogs"
        }
      ]
    };
  }
};
</script>
