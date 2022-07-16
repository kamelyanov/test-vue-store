<template>
  <section class="container">
    <div class="sort"></div>
    <div class="cards">
      <Card
        image="https://mykitai.ru/wp-content/uploads/2019/03/Velikaya-Kitajskaya-stena-1.jpg"
        name="Название товара"
        about="ДЛинное описание товара из несокльких строк несколько раз по длинному описанию чтобы очень интересно было читать всем"
        price="Цена товара"
      />
      <Card
        image="https://mykitai.ru/wp-content/uploads/2019/03/Velikaya-Kitajskaya-stena-1.jpg"
        name="Название товара"
        about="ДЛинное описание товара из несокльких строк несколько раз по длинному описанию чтобы очень интересно было читать всем"
        price="Цена товара"
      />
      <Card
        image="https://mykitai.ru/wp-content/uploads/2019/03/Velikaya-Kitajskaya-stena-1.jpg"
        name="Название товара"
        about="ДЛинное описание товара из несокльких строк несколько раз по длинному описанию чтобы очень интересно было читать всем"
        price="Цена товара"
      />
    </div>
  </section>
</template>

<script>
  import Card from './Card'
  export default {
    props:['card'],
    components: {
      Card
  },
}
</script>
