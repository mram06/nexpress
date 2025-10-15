<template>
  <header class="header">
    <div class="container">
      <div class="header__body">
        <div class="header__top">
          <NuxtLink to="/">
            <img src="~/assets/img/logo.png" alt="logo" />
          </NuxtLink>
          <div class="header__info">
            <div class="header__info-phone">0 800 000 000</div>
            <div class="header__info-name text">контакт-центр</div>
            <div class="header__info-email text">nextexpress@nexpress.ua</div>
          </div>
        </div>
        <div class="header__bottom">
          <Navbar />
          <div>UA</div>
        </div>
      </div>
    </div>
  </header>
</template>

<script setup lang="ts">
import Navbar from "./Navbar.vue";
</script>

<style lang="scss" scoped>
.header {
  &__body {
    @include app-container;
  }

  &__top {
    padding: 16.5px 0;

    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  &__info {
    text-align: end;
    &-phone {
      font-size: 14px;
    }
    &-name {
      font-size: 14px;
    }
    &-email {
      font-size: 14px;
    }
  }

  &__bottom {
    padding: 8px 0;

    display: flex;
    justify-content: space-between;
    align-items: center;
  }
}
</style>
