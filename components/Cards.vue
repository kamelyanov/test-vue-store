<template>
  <section class="container">
    <div class="sort"></div>
    <div class="cards">
      <Card
        image="https://mykitai.ru/wp-content/uploads/2019/03/Velikaya-Kitajskaya-stena-1.jpg"
        name="Название товара"
        about="Довольно-таки интересное описание товара в несколько строк. Довольно-таки интересное описание товара в несколько строк"
        price="10 000 руб."
      />
      <Card
        image="https://mykitai.ru/wp-content/uploads/2019/03/Velikaya-Kitajskaya-stena-1.jpg"
        name="Название товара"
        about="Довольно-таки интересное описание товара в несколько строк. Довольно-таки интересное описание товара в несколько строк"
        price="10 000 руб."
      />
      <Card
        image="https://mykitai.ru/wp-content/uploads/2019/03/Velikaya-Kitajskaya-stena-1.jpg"
        name="Название товара"
        about="Довольно-таки интересное описание товара в несколько строк. Довольно-таки интересное описание товара в несколько строк"
        price="10 000 руб."
      />
            <Card
        image="https://mykitai.ru/wp-content/uploads/2019/03/Velikaya-Kitajskaya-stena-1.jpg"
        name="Название товара"
        about="Довольно-таки интересное описание товара в несколько строк. Довольно-таки интересное описание товара в несколько строк"
        price="10 000 руб."
      />
            <Card
        image="https://mykitai.ru/wp-content/uploads/2019/03/Velikaya-Kitajskaya-stena-1.jpg"
        name="Название товара"
        about="Довольно-таки интересное описание товара в несколько строк. Довольно-таки интересное описание товара в несколько строк"
        price="10 000 руб."
      />
            <Card
        image="https://mykitai.ru/wp-content/uploads/2019/03/Velikaya-Kitajskaya-stena-1.jpg"
        name="Название товара"
        about="Довольно-таки интересное описание товара в несколько строк. Довольно-таки интересное описание товара в несколько строк"
        price="10 000 руб."
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

<style>
  .cards {
    display: flex;
    flex-wrap: wrap;
    gap: 16px;
  }
</style>
