<template>
  <div id="app">
    <Header @HandleLinkSelection="NavigateTo"/>
    <Body/>
    <Footer/>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Body from "./components/Body.vue";
import Footer from "./components/Footer.vue";
export default {
  name: "App",
  components: {
    Header,
    Body,
    Footer
  },
  methods: {
    NavigateTo(selection) {
	console.log(selection);
	}
  }
};
</script>

<style>
</style>
