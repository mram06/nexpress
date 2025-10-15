<template>
  <nav class="menu text">
    <ul>
      <li>
        <NuxtLink>Трекінг</NuxtLink>
      </li>
      <li><NuxtLink>Розрахувати вартість</NuxtLink></li>
      <li><NuxtLink>Оформити</NuxtLink></li>
      <li><NuxtLink>Тарифи</NuxtLink></li>
      <li><NuxtLink>Відділення</NuxtLink></li>
      <li><NuxtLink>Про нас</NuxtLink></li>
    </ul>
  </nav>
</template>

<script setup lang="ts"></script>

<style scoped>
ul {
  display: flex;
  align-items: center;
  gap: 32px;
}
</style>
