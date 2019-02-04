<template>
  <div>
    <h2>/users/_id.vue</h2>
    <p>User ID: {{userId}}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      userId: this.$route.params.id
    };
  }
};
</script>
