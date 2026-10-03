<template>
  <div class="student-card">
    <h1>Страница студента</h1>
    <ul>
      <li><strong>Имя:</strong> {{ name }}</li>
      <li><strong>Возраст:</strong> {{ age }}</li>
      <li><strong>Город:</strong> {{ city }}</li>
      <li><strong>Направление обучения:</strong> {{ direction }}</li>
    </ul>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const name = ref('Антон Мухов')
const age = ref(21)
const city = ref('Краснодар')
const direction = ref('Прогромирования')
</script>

<style scoped>
.student-card {
  max-width: 400px;
  margin: 40px auto;
  padding: 24px;
  border: 1px solid #000000;
  border-radius: 12px;
  font-family: sans-serif;
  background: #000000;
}
.student-card h1 {
  font-size: 1.4rem;
  margin-bottom: 16px;
}
.student-card ul {
  list-style: none;
  padding: 0;
}
.student-card li {
  padding: 8px 0;
  border-bottom: 1px solid #020202;
}
.student-card strong {
  display: inline-block;
  width: 200px;
}
</style>
