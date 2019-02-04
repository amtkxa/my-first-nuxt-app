<template>
  <div>
    <h2>/users/index.vue</h2>
  </div>
</template>

<script>
export default {
  async mounted() {
    console.log(
      JSON.stringify(
        // Qiita API から、Nuxt.js のタグが付けられた投稿を取得する。
        await this.$axios.$get(
          "https://qiita.com/api/v2/items?query=tag:nuxt.js"
        ),
        true,
        " "
      )
    );
  }
};
</script>
