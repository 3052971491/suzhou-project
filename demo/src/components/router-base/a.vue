<template>
  <div>
    这是a页面
    <router-link to="/b">跳转到b页面</router-link>
    <button @click="TiaoA">按钮跳转到b页面</button>
    <button @click="GetAsg">获取传参</button>
  </div>
</template>
<script>
import AChild from "./a-child";
export default {
  data() {
    return {
      test: "传入组件内部参数",
    };
  },
  methods: {
    TiaoA() {
      console.log(22);
      this.$router.push({ path: "/b" });
    },
    GetAsg() {
      console.log(this.$route.query);
    },
  },
};
</script>
