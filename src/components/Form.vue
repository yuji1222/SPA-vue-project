<template>
  <div class="form container">
    <div class="formarea">
      <form>
        <div class="form-group">
          <label for="exampleFormControlInput1">お名前</label>
          <input type="text" class="form-control form-control-sm" id="exampleFormControlInput1" />
        </div>
        <div class="form-group">
          <label for="exampleFormControlInput1">貴社名</label>
          <input type="text" class="form-control form-control-sm" id="exampleFormControlInput1" />
        </div>
        <div class="form-group">
          <label for="exampleFormControlInput1">メールアドレス</label>
          <input type="email" class="form-control form-control-sm" id="exampleFormControlInput1" />
        </div>
        <div class="form-group">
          <label for="exampleFormControlInput1">電話番号</label>
          <input type="number" class="form-control form-control-sm" id="exampleFormControlInput1" />
        </div>
        <div class="form-group">
          <label for="exampleFormControlTextarea1">問い合わせ内容</label>
          <textarea class="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>
        </div>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: "Form"
};
</script>

<style scoped>
.form-group {
  width: 300px;
}
</style>