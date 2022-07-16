<template>
  <div class="addForm">
    <h2 class="addForm__title">Добавление товара</h2>
    <form class="form" @submit.prevent="handleSubmit">
      <FormInput
        inputName='Наименование товара'
        placeholder="Введите наименование товара"
        name="name"
        required="required"
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
        required="required"
      />

      <FormInput
        inputName='Цена товара'
        placeholder="Введите цену"
        name="price"
        required="required"
      />

      <button
        class="button__confirm"
        type="submit"
      >
      Добавить товар
      </button>

    </form>


  </div>
</template>

<script>
import FormInput from './FormInput'

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
      FormInput
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

</style>
