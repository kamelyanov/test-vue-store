<template>
  <button class="button__confirm" type="submit">Добавить товар</button>
</template>

<style lang="scss">
  .button__confirm {
    width: 284px;
    height: 36px;
    color: var(--white);
    font-size: 12px;
    line-height: 36px;
    background-color: var(--btn-cf-background);
    border: none;
    border-radius: var(--btn-cf-br);
    box-shadow: var(--btn-cf-bs);
    cursor: pointer;
    transition: 300ms;

  &__confirm:hover {
    box-shadow: var(--inputs-shadow-hover);
  }

   &__confirm:active {
    transform: scale(0.99);
  }
}

</style>
