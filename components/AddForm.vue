<template>
  <div class="addForm">
    <h2 class="addForm__title">Добавление товара</h2>
    <form class="form" @submit.prevent="handleSubmit">
      <FormInput
        inputName='Наименование товара'
        placeholder="Введите наименование товара"
        name="name"
        required
      />

      <FormInput
        inputName='Описание товара'
        placeholder="Введеите описание товара"
        name="about"
      />

      <FormInput
        inputName='Ссылка на изображение товара'
        placeholder="Введите ссылку"
        name="image"
        required
      />

      <FormInput
        inputName='Цена товара'
        placeholder="Введите цену"
        name="price"
        required
      />

      <ButtonConfirm/>

    </form>

  </div>
</template>

<script>
import FormInput from './FormInput'
import ButtonConfirm from './ButtonConfirm.vue'

function initialState() {
  return {
    name: '',
    about: '',
    image: '',
    price: '',
  }
}

export default {
  data: initialState,
  components: {
      FormInput, ButtonConfirm
    },
  methods: {
     handleSubmit() {
      const {name, about, image, price} = this
      this.$emit('submit', {
        name: name,
        about: about,
        image: image,
        price: price,
      })
    Object.assign(this.$data, initialState())
    console.log(this.$data)
    }
  },
  emits: ['submit'],
}
</script>

<style>
  .addForm__title {
    font-size: 28px;
    line-height: 36px;
    font-weight: 600;
    white-space: nowrap;
  }

  .form {
    padding: 24px;
    width: 332px;
    display: flex;
    flex-direction: column;
    gap: 16px;
    background-color: var(--cards-background);
    box-shadow: var(--cards-shadow);
    border-radius: var(--cards-border-radius);
  }
</style>
