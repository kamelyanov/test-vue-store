<template>
  <label class="input">
    <p class="input__name">{{ inputName }}</p>
    <input
      class="input__value"
      :placeholder="placeholder"
      type="text"
      :name="name"
    />
  </label>
</template>

<script>
export default {
  props: ['placeholder', 'name', 'inputName']
}
</script>

<style lang="scss" scoped>
  .input {
    display: flex;
    flex-direction: column;
    gap: 4px;

    &__name {
      font-size: 10px;
      line-height: 13px;
      color: #49485E;
    }

    &__value {
      border: none;
      box-shadow: var(--inputs-shadow);
      color: var(--inputs-color-name);
      padding: 10px 16px;
    }

    &__value::placeholder{
      font-weight: 400;
      font-size: 12px;
      line-height: 15px;
      color: var(--inputs-color-ph);
    }

    &__value:focus {
      border: 1px solid #555;
    }
  }



</style>
