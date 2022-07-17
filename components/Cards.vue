<template>
  <section class="container">
    <div class="sort">
      <select class="sort__select">
        <option class="sort__option">По умолчанию</option>
        <option class="sort__option">По цене min</option>
        <option class="sort__option">По цене max</option>
        <option class="sort__option">По наименованию</option>
      </select>
    </div>
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
import Card from "./Card";
export default {
  props: ["card"],
  components: {
    Card,
  },
};
</script>

<style>
  .container {
    display: flex;
    flex-direction: column;
    gap: 16px;
  }

  .cards {
    display: flex;
    flex-wrap: wrap;
    gap: 16px;
  }

  .sort {
    align-self: end;
  }

  .sort__select {
    position: relative;
    height: 36px;
    padding: 10px 27px 10px 16px;
    font-size: 12px;
    line-height: 15px;
    color: var(--inputs-color-ph);
    border-radius: var(--cards-border-radius);
    border: none;
    box-shadow: var(--inputs-shadow-hover);
    background: var(--cards-background) url(@/assets/icons/sort-arrow.svg) 90% center no-repeat;
    -webkit-appearance: none;
    -moz-appearance: none;
    appearance: none;
  }
</style>
