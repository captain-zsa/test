<template>
  <div class="layout">
    <div class="layout__button">
      <AppButton
        href="#"
        is-button-fill
        disabled
        color="primary"
        icon="plus"
        icon-position="right"
        icon-color="white"
      >
        Текст
      </AppButton>
    </div>
  </div>
</template>

<script>
export default {
  name: 'AppLayout'
};
</script>

<style lang="scss" scoped>
.layout {
  &__button {
    width: 200px;
  }
}
</style>
