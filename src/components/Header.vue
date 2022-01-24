<template>
  <!-- Content in this component, things you will export -->
  <header>
    <h1>Task Tracker</h1>
  </header>
</template>

<script>
// * JS logic about this component, define export first
export default {
  name: 'Header',
};
</script>

<style scoped>
/* scoped means anything in here will be only used for this component particular. */
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}
</style>
