<template>
  <div class="card mb-3">
    <div class="card-body">
      <h4 v-if="props.title">{{ props.title }}</h4>

      <p>{{ props.content }}</p>

      <small class="text-muted">โพสต์โดย คนที่คุณก็รู้ว่าใคร...</small>
    </div>
  </div>
</template>
<script setup>
import { defineProps } from "vue";
const props = defineProps({
  content: String
});
</script>
