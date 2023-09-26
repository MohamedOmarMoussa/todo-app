<script setup lang="ts">
import { TodoStatus } from "@/types";
import TodoGroup from "./TodoGroup.vue"
</script>

<template>
  <div class="group-wrapper">
    <TodoGroup :status="TodoStatus.Pending"/>
    <TodoGroup :status="TodoStatus.InProgress"/>
    <TodoGroup :status="TodoStatus.Completed"/>
  </div>
</template>

<style scoped>
  .group-wrapper {
    display: flex;
    justify-content: space-around;
    gap: 20px;
  }
</style>
