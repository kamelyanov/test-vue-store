<template>
  <div class="card">
    <img class="card__image"
      :src="image" :alt="name"
    />
    <div class="card__info">
      <p class="info__name"> {{name}} </p>
      <p class="info__about"> {{about}} </p>
      <p class="info__price"> {{price}} </p>
    </div>
    <button class="card__delete"
    />
  </div>
</template>

<script>
export default {
  props: ['image', 'name', 'about', 'price', 'id'],
}
</script>

<style>
  .card {
    height: 423px;
    width: 332px;
    background-color: var(--cards-background);
    box-shadow: var(--cards-shadow);
    border-radius: var(--cards-border-radius);
    position: relative;
    cursor: pointer;
  }

  .card__image{
    height: 200px;
    width: 332px;
    border-radius: var(--cards-border-radius) var(--cards-border-radius) 0 0;
    object-fit: cover;
  }

  .card__info{
    padding: 16px 24px;
    color: var(--cards-text-color);
  }

  .info__name {
    font-size: 20px;
    line-height: 25px;
    font-weight: 600;
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
  }

  .info__about {
    margin-top: 16px;
    margin-bottom: 32px;
    height: 80px;
    font-weight: 400;
    font-size: 16px;
    line-height: 20px;
    overflow: hidden;
    text-overflow: ellipsis;
    display: -webkit-box;
    -webkit-line-clamp: 5;
    -webkit-box-orient: vertical;
  }

  .info__price {
    font-weight: 600;
    font-size: 24px;
    line-height: 30px;
  }

  .card__delete{
    opacity: 0;
    position: absolute;
    background: transparent;
    border: none;
    background-image: url(@/assets/icons/delete-button.svg);
    background-repeat: no-repeat;
    background-size: 100%;
    height: 32px;
    width: 32px;
    cursor: pointer;
    top: -8px;
    right: -8px;
    border-radius: 10px;
    transition: 0.2s;
  }

  .card__delete:hover {
    transform: scale(1.1)
  }

   .card__delete:active {
    transform: scale(0.9)
  }

  .card:hover .card__delete {
    opacity: 1;
  }
</style>
