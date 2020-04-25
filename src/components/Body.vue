<template>
  <div id="BodyContainer">
    <ServiceContainer/>
    <MapContainer/>
    <TestimonialContainer/>
    <FormContainer/>
  </div>
</template>

<script>
import ServiceContainer from "./BodyComponents/ServiceContainer.vue";
import MapContainer from "./BodyComponents/MapContainer.vue";
import TestimonialContainer from "./BodyComponents/TestimonialContainer.vue";
import FormContainer from "./BodyComponents/FormContainer.vue";

export default {
  name: "Body",
  components: {
    ServiceContainer,
    MapContainer,
    TestimonialContainer,
    FormContainer
  },
  data() {
    return {
      a: ""
    };
  }
};
</script>
