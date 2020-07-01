<template>
  <li class="main__item">
    <a href="">
      <span>{{ nav.title }}</span>
    </a>
  </li>
</template>

<script>
export default {
  props: {
    nav: {
      type: Object,
      required: true,
    }
  }
}
</script>