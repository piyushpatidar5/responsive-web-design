<template>
  <div id="FormContainer">
    <div class="MaginAuto">
      <div class="FormHeadingContainer WHiteLabel text-align-center">
        <h2>Convinced To Work With Us?</h2>
        <span
          class="InfoLabel"
        >Company has helped agencies keep their promises to client since 2005.</span>
      </div>
      <div class="FormBox">
        <form onsubmit.prevent="handleSubmitAction()">
          <div class="InputContainer">
            <input placeholder="Fullname">
            <input placeholder="Email Adress">
            <input placeholder="Phone Number">
          </div>
          <div class="TextBoxContainer">
            <textarea placeholder="Message in brief"></textarea>
          </div>
          <div class="SubmitContainer">
            <input class="SubmitButton RoundBorderContainer" type="submit">
          </div>
        </form>
      </div>
    </div>
  </div>
</template>


<script>
export default {
  name: "FormContainer",
  components: {},
  methods: {
    handleSubmitAction() {
      // Handles formSubmit
    }
  }
};
</script>
