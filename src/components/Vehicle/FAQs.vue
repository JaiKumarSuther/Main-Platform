<script setup>
import { ref } from 'vue'

const props = defineProps({
  items: {
    type: Array,
    default: () => []
  }
})

const openIndex = ref(null)

const toggle = (index) => {
  openIndex.value = openIndex.value === index ? null : index
}
</script>

<template>
  <div class="questions">
    <h2>Questions you may have</h2>
    <ul class="question-list">
      <li v-for="(item, index) in items" :key="index">
        <div class="question-list-item" @click="toggle(index)">
          <img src="/src/images/Faq icon.svg" alt="" />
          <div class="question-list-text">
            <h3>{{ item.question }}</h3>
            <p v-if="openIndex === index">{{ item.answer }}</p>
          </div>
          <img
            :src="openIndex === index
              ? '/src/images/toggle up.svg'
              : '/src/images/dropdown toggle.svg'"
            alt="Toggle Icon"
            class="toggle-icon"
          />
        </div>
      </li>
    </ul>
  </div>
</template>
