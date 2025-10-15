<template>
  <footer class="footer">
    <div class="container">
      <div class="footer__body">
        <div class="footer__top">
          <NuxtLink to="/">
            <img src="~/assets/img/logo.png" alt="logo" />
          </NuxtLink>

          <ul class="footer__links text">
            <li>
              <NuxtLink>Умови використання</NuxtLink>
            </li>
            <li><NuxtLink>Повідомлення про конфіденційність</NuxtLink></li>
            <li><NuxtLink>Додаткова інформація</NuxtLink></li>
            <li><NuxtLink>Контакти</NuxtLink></li>
          </ul>
        </div>
        <div class="footer__bottom"></div>
      </div>
    </div>
  </footer>
</template>

<script setup lang="ts"></script>

<style lang="scss" scoped>
.footer {
  &__body {
    @include app-container;
    padding-top: 32px;
    padding-bottom: 32px;
  }

  &__top {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  &__links {
    display: flex;
    align-items: center;
    gap: 32px;

    font-size: 14px;
  }

  &__bottom {
  }
}
</style>
