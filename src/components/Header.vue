<template>
  <div class="HeaderContainer">
    <div class="MaxWidthContainer DisplayFlexBox">
      <div class="WHiteLabel IconContainer">
        <i class="fas fa-align-justify"></i>
      </div>
      <div id="LogoContainer" class="VerticallyAlignMiddleChild">
        <span class="LogoLabel WHiteLabel">COMPANY</span>
        <span class="OrangeLabel LogoLabel padding-left-5">LOGO</span>
      </div>
      <div id="LinksContainer" class="VerticallyAlignMiddleChild">
        <span
          :key="index"
          v-for="(link,index) in links"
          :class="link.label==selected.label?'Selected padding-right-20 padding-left-20':'UnSelected padding-right-20 padding-left-20'"
          @click="handleSelection(link)"
        >{{link.label}}</span>

        <div class="DisplayInlineFlex margin-left-20">
          <div
            class="RoundBorderContainer padding-right-20 padding-left-20 padding-top-10 padding-bottom-10"
          >
            <i class="CommentIcon WHiteLabel far fa-comment-alt VerticallyAlignMiddleChild"></i>
            <span class="WHiteLabel padding-left-10 VerticallyAlignMiddleChild">Get In Touch</span>
          </div>
        </div>
      </div>
      <div class="WHiteLabel IconContainer">
        <i class="far fa-comment-alt"></i>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
  components: {},
  data() {
    return {
      links: [
        {
          label: "About",
          navigateTo: ""
        },
        {
          label: "Services",
          navigateTo: ""
        },
        {
          label: "Solutions",
          navigateTo: ""
        },
        {
          label: "Blog",
          navigateTo: ""
        }
      ],
      selected: {
        label: "About",
        navigateTo: ""
      }
    };
  },
  methods: {
    handleSelection(selected) {
      this.selected = selected;
      this.$emit("HandleLinkSelection", selected);
    }
  }
};
</script>

<style>
</style>
