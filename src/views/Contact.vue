<template>
  <div class="contact container">
    <h1 class="mb-5">Contact</h1>
    <p class="md-5">
      制作の依頼・ご相談などお気軽にお問い合わせくださいませ。
      <br />下記フォームよりわかる範囲でご記入ください。
      <br />必須の項目は必ずご記入お願いします。
    </p>
    <Form></Form>
  </div>
</template>

<script>
import Form from "@/components/Form.vue";

export default {
  name: "contact",
  components: {
    Form
  }
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css?family=Mansalva|Noto+Serif+JP&display=swap");

* {
  font-family: "Mansalva", cursive;
  font-family: "Noto Serif JP", serif;
}
</style>