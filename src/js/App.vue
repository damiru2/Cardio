<template>
  <div>{{ text }}</div>
</template>

<script>
export default {
  data() {
    return {
      text: 'Hello there, Guys!',
    };
  },
};
</script>

<style lang="scss">
$bgColor: red;

div {
  background: $bgColor;
}
</style>
