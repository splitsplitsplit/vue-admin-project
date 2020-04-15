<template>
  <div>
    <a-form layout="horizontal">
      <a-form-item label="密码">
        <a-input type="password" placeholder="请输入密码"></a-input>
      </a-form-item>
    </a-form>
    <a-button type="primary" @click="onPrev">上一步</a-button>
    <a-button style="margin-left:8px" type="primary" @click="handleSubmit">提交</a-button>
  </div>
</template>

<script>
export default {
  methods: {
    handleSubmit() {
      this.$router.push("/form/step-form/result");
    },
    onPrev() {
      this.$router.push("/form/step-form/info");
    }
  }
};
</script>

<style></style>
