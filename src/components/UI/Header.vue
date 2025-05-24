<script setup>
defineProps({
  location: {
    type: String,
    required: true
  }
})
</script>

<template>
  <div class="header">
    <span class="location">
      <img src="/src/images/Location icon.svg" alt="" /> {{ location }}
    </span>
  </div>
</template>
