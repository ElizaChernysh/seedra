<template>
  <div class="container">
    <div class="header">
      <a href="">
        <img src="../../image/logo.svg" />
      </a>

      <div class="header__desktop">
        <nav>
          <ul class="header__nav">
            <li class="header__item">
              <a class="header__links" href="">ALL PRODUCTS</a>
            </li>
            <li class="header__item">
              <a class="header__links" href="">ABOUT SEEDRA</a>
            </li>
            <li class="header__item">
              <a class="header__links" href="">OUR BLOG</a>
            </li>
            <li class="header__item">
              <a class="header__links" href="">CONTACTS</a>
            </li>
          </ul>
        </nav>

        <div class="header__media">
          <a class="header__media-links">
            <img src="../../image/icons/instagram.svg" alt="link to instagram" />
          </a>
          <a class="header__media-links">
            <img src="../../image/icons/facebook.svg" alt="link to facebook" />
          </a>
        </div>

        <form class="header__form">
          <img class="header__form-img" src="../../image/input/search.svg" />
          <input class="header__input" type="text" placeholder="Search" />
        </form>

        <div class="">    
          <a class="header__actions-links">
            <img class="" src="../../image/icons/max-heart.svg"/>
          </a>
          <a class="header__actions-links">
            <img class="" src="../../image/icons/max-basket.svg"/>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>
}

<script>
export default {
  name: 'navbar-header'
}
</script>

<style lang="scss" scoped>
@import "@/styles/_variables.scss";


.header {
  display: flex;
  justify-content: space-between;
  align-items: center;

  &__desktop {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  &__nav {
    display: flex;
  }

  &__item {
    &:not(:last-child) {
      border-right: 1px solid #efefef;
      margin-right: 16px;
    }
  }

  &__links {
    color: $color-text-gray;
    padding-right: 16px;
  }

  &__media-links:not(:last-child) {
    margin-right: 12px;
  }

  &__media {
    display: flex;
    margin-right: 15px;
  }

  &__form {
    width: 285px;
    border: 1px solid #efefef;
    border-radius: 71px;
    padding: 0 24px;
    display: flex;
    margin-right: 15px;
  }

  &__form-img {
    margin-right: 16px;
  }

  &__input {
    border: none;
    font-size: 14px;
    line-height: 178.19%;
    height: 48px;
    // padding: 0 20px;
    outline: none;
  }

  &__actions-links {
    &:not(:last-child) {
      margin-right: 28px;
    }
  }
}
</style>