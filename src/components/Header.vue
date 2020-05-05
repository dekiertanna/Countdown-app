<template>
  <div>
    <md-toolbar>
      <h3 class="md-title">The final countdown!</h3>
    </md-toolbar>
  </div>
</template>

<script>
export default {
  name: "Layout",
};
</script>

<style lang="scss" scoped>
.md-toolbar + .md-toolbar {
  position: fixed;
  padding: 0px;
}
</style>
