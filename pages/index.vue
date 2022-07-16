<template>
  <div class="main">
    <AddForm/>
    <Cards/>
  </div>
</template>

<script>
  import AddForm from '@/components/AddForm.vue'
  import Cards from '@/components/Cards.vue'

  export default {
    name: 'App',
    components: {
      AddForm, Cards
    }
  }
</script>
