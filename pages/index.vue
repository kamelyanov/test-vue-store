<template>
  <div class="root">
    <div class="main">
      <AddForm/>
      <Cards/>
    </div>
  </div>
</template>

<script>
  import AddForm from '@/components/AddForm.vue'
  import Cards from '@/components/Cards.vue'

  export default {
    components: {
      AddForm, Cards
    }
  }
</script>

<style>
  .root{
    background-color: var(--page-background);
    height: 100vh;
  }

  .main{
    display: flex;
    flex-direction: row;
    gap: 16px;
    padding: 32px;
    min-height: 100%;
    max-width: 1440px;
    margin: 0 auto 0;
  }
</style>
