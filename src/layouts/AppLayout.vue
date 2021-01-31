<template>
  <div class="layout">
    <div class="layout__button">
      <AppButton
        type="button"
        fill
        color="silver"
        icon="plus"
        icon-position="right"
        icon-color="black"
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
