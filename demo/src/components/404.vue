<template>
  <div>
    <button @click="goBack">返回</button>
    <h1>Not Found</h1>
    <h6>The requested URL /a was not found on this server.</h6>
  </div>
</template>

<script>
export default {
  methods: {
    goBack() {
      this.$router.go(-1);
    },
  },
};
</script>