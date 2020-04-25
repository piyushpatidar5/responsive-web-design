<template>
  <div id="TestimonialContainer">
    <div id="MainConatiner">
      <div class="HeadingContainer text-align-center">
        <h2>Testimonials</h2>
      </div>
      <div class="CardsContainer DisplayFlexBox">
        <div class="CommentNode" :key="index" v-for="(node, index) in CommentNodes">
          <CardsContainer :nodeData="node"/>
        </div>
      </div>
    </div>
  </div>
</template>


<script>
import CardsContainer from "./TestimonialComponents/CardsContainer.vue";
export default {
  name: "TestimonialContainer",
  components: { CardsContainer },
  data() {
    return {
      CommentNodes: [
        "Contrary to popular belief, Lorem Ipsum is not simply random text. It has roots in a piece of classical Latin literature from 45 BC, making it over 2000 years old.",
        " Richard McClintock, a Latin professor at Hampden-Sydney College in Virginia, looked up one of the more obscure Latin words, consectetur, from a Lorem Ipsum passage, and going through the cites of the word in classical literature, discovered the undoubtable source.",
        "Richard McClintock, a Latin professor at Hampden-Sydney College in Virginia, looked up one of the more obscure Latin words, consectetur, from a Lorem Ipsum passage."
      ]
    };
  }
};
</script>
