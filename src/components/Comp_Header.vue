<script setup>

import Logo from '@/components/elements/Ele_Logo.vue'
import Menu from '@/components/elements/Ele_Menu.vue'
import Search from '@/components/elements/Ele_Search.vue'

</script>

<template>
  <header class="header">
    <div class="header__content">
      <Logo class="header__content__logo" />
      <Menu />
      <Search />
    </div>
  </header>
</template>

<style lang="scss" scoped>
.header {
  z-index: 50;
  position: sticky;
  top: 0;
  display: block;
  width: 100vw;
  margin-top: 15px;
  background: $color-white;

  &__content {
    max-width: 85vw;
    margin: auto;
    padding: 15px 0;
    display: flex;
    justify-content: space-between;
    align-items: center;

    &__logo {
      display: block;
      width: 100px;
    }
  }
}
</style>