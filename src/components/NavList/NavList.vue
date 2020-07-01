<template>
  <nav class="header__nav">
    <ul>
      <NavItem
        v-for="nav of navs"
        v-bind:nav="nav"
      />
    </ul>
  </nav>
</template>

<script>
import NavItem from '@/components/NavItem/NavItem'
export default {
  props: ['navs'],
  components: {
    NavItem
  }
}
</script>

<style lang="scss">
  @import './NavList.module.scss';
</style>
