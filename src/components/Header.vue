<template>
  <!-- Content in this component, things you will export -->
  <header>
    <h1>{{ title }}</h1>
    <Button
      @btn-click="$emit('toggle-add-task')"
      :text="showAddTask ? 'Close' : 'Add Task'"
      :color="showAddTask ? 'red' : 'green'"
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
    showAddTask: Boolean,
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
