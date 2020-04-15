<template>
  <div>
    <a-form layout="horizontal">
      <a-form-item label="账号">
        <a-input placeholder="请输入账号"></a-input>
      </a-form-item>
    </a-form>
    <a-button type="primary" @click="handleSubmit">下一步</a-button>
  </div>
</template>

<script>
export default {
  methods: {
    handleSubmit() {
      this.$router.push("/form/step-form/confirm");
    }
  }
};
</script>

<style></style>
