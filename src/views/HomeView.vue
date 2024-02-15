<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
  </div>
</template>

<script lang="ts">
import { defineComponent, reactive } from 'vue';
import Todo from '@/components/Todo.vue';
import type TodoType from '@/types/TodoType';

const Todos = reactive<TodoType[]>([]);

export default defineComponent({
  name: 'HomeView',
  components: {
    Todo,
  },
});
</script>
