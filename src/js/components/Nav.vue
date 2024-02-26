<template>
  <nav class="nav">
    <span class="nav__logo">WORKOUT</span>
    <ul class="nav__links">
      <li><a href="">УПРАЖНЕНИЯ</a></li>
      <li><a href="">ТРЕНИРОВКИ</a></li>
      <li><a href="">ЦЕНЫ</a></li>
      <li><a href="">ПРО НАС</a></li>
    </ul>
  </nav>
</template>

<script>
export default {};
</script>

<style lang="scss">
.nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 50px;

  .nav__logo {
    font-size: 1.8em;
    text-transform: uppercase;
  }

  .nav__links {
    list-style: none;
    text-transform: uppercase;

    > li {
      display: inline-block;

      &:not(:last-of-type) {
        margin-right: 27px;
      }
    }
  }
}
</style>
