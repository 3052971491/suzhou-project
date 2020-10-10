<template>
  <div>
    这是b页面
    <router-link to="/a">跳转到a页面</router-link>
    <button @click="TiaoA">按钮跳转到a页面</button>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  methods: {
    TiaoA() {
      console.log(11);
      //   区别  类似get请求post请求
      //   this.$router.push({
      //     path: "/a",
      //     query: { name: "tom", age: "10", height: "180" },
      //   });
      this.$router.push({
        name: "a",
        params: { name: "tom", age: "10", height: "180" },
      });
    },
  },
};
</script>