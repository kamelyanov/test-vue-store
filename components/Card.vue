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