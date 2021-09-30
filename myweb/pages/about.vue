<template>
  <div>
    <h1>我來自 {{ name }} 端</h1>
    <nuxt-link to="/">回到首頁</nuxt-link>
  </div>
</template>
<script>
export default {
  layout: "default",
  data({ req }) {
    return {
      name: req ? "server" : "client"
    };
  }
};
</script>
