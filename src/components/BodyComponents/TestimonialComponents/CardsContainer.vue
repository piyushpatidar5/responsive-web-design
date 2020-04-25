<template>
  <div>
    <div class="CommentNodeContainer">{{nodeData}}</div>
    <div class="triangle-with-shadow"></div>
    <div class="ClientNameContainer">
      <div class="CircleContainer">
        <i class="PersonIcon fas fa-user-alt"></i>
      </div>
      <div class="LableContainer">
        <span class="HeadingLabel">CLIENT NAME</span>
        <br>
        <span class="PositionLabel">Position, ORG</span>
      </div>
    </div>
  </div>
</template>


<script>
export default {
  name: "CardsContainer",
  components: {},
  props: ["nodeData"],
  data() {
    return {
      a: ""
    };
  }
};
</script>
