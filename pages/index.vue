<template>
  <div class="hero">
    <div class="container">
      <div class="hero__body">
        <h1 class="hero__title">
          Розширюємо мережу: нові відділення в кожному регіоні!
        </h1>
        <div class="hero__map"></div>
        <div class="hero__buttons">
          <button>
            <img src="~/assets/icons/files.svg" /> Розрахувати вартість
          </button>
          <button><img src="~/assets/icons/add.svg" /> Оформити</button>
          <button><img src="~/assets/icons/location.svg" /> Відділення</button>
        </div>
      </div>
    </div>
  </div>

  <div class="services">
    <div class="container">
      <div class="services__body">
        <h2 class="services__title">Наші послуги</h2>
        <div class="services__items">
          <div class="services__item">
            <p class="services__item-title">Авіаперевезення</p>
            <div class="services__item-img">
              <img src="~/assets/icons/airplane.svg" alt="service img" />
            </div>
          </div>
          <div class="services__item">
            <p class="services__item-title">Доставка документів</p>
            <div class="services__item-img">
              <img src="~/assets/icons/truck.svg" alt="service img" />
            </div>
          </div>
          <div class="services__item">
            <p class="services__item-title">Міжнародна доставка</p>
            <div class="services__item-img">
              <img src="~/assets/icons/packages.svg" alt="service img" />
            </div>
          </div>
          <div class="services__item">
            <p class="services__item-title">Доставка по Україні</p>
            <div class="services__item-img">
              <img src="~/assets/icons/truck_packages.svg" alt="service img" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <div class="slider">
    <div class="container">
      <div class="slider__body">
        <h2 class="slider__title">Доставка за ніч - розгінемо час!</h2>
        <p class="slider__text text">
          Тепер ваші важливі відправлення можуть бути у відділенні Next Express
          вже наступного ранку! Оберіть послугу доставки за ніч та отримайте
          гарантовану швидкість та надійність.
        </p>
        <button class="slider__button">Дізнатись більше</button>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts"></script>

<style lang="scss" scoped>
.hero {
  &__body {
    @include app-container();
    position: relative;

    padding-top: 162px;
    padding-bottom: 32px;

    background: linear-gradient(
      135deg,
      #8b5fbf 0%,
      #6b73ff 25%,
      #4fc3f7 50%,
      #81d4fa 75%,
      #b3e5fc 100%
    );
  }
  &__map {
    position: absolute;
    top: 65px;
    right: 123px;

    height: 100%;
    width: 528px;
    height: 362px;
    background: url("~/assets/img/map.png") no-repeat;
  }

  &__title {
    max-width: 477px;
  }

  &__buttons {
    margin: 162px 0 0 0;

    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 30px;

    button {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 8px;

      border-radius: 8px;
      background: rgb(1, 79, 171);
      color: rgb(255, 255, 255);
      font-size: 16px;
      font-weight: 500;
      line-height: 120%;
      letter-spacing: 0%;
      text-wrap: nowrap;

      width: 100%;
      padding: 16px;
    }
  }
}

.services {
  &__body {
    @include app-container();
    padding-top: 96px;
    padding-bottom: 96px;
  }

  &__title {
  }
  &__items {
    margin: 24px 0 0 0;

    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 30px;
  }
  &__item {
    display: flex;
    flex-direction: column;
    gap: 40px;
    align-items: center;
    padding: 38px;

    width: 276px;
    height: 276px;

    background-color: white;
    &-title {
    }
    &-img {
      display: flex;
      align-items: center;

      height: 111px;
      img {
        width: 100%;
      }
    }
  }
}

.slider {
  &__body {
    @include app-container;
    padding-top: 124px;
    padding-bottom: 124px;

    background: rgb(1, 79, 171);
  }

  &__title {
    color: white;
    max-width: 582px;
  }

  &__text {
    margin-top: 16px;

    color: rgba(255, 255, 255, 0.8);
    max-width: 582px;
  }

  &__button {
    margin-top: 40px;

    display: flex;
    align-items: center;
    justify-content: center;
    gap: 8px;

    border-radius: 8px;
    background: white;

    font-size: 16px;
    font-weight: 500;
    line-height: 120%;
    letter-spacing: 0%;
    text-wrap: nowrap;

    width: 100%;
    max-width: 276px;
    padding: 16px;
  }
}
</style>
