<template>
  <!-- Content in this component, things you will export -->
  <header>
    <h1>{{ title }}</h1>
    <Button
      @toggle-add-task="$emit('toggle-add-task')"
      text="Add Task"
      color="green"
    />
  </header>
</template>

<script>
import Button from './Button.vue';
export default {
  name: 'Header',
  components: {
    Button,
  },
  props: {
    title: String,
  },
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
