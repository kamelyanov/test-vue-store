<template>
  <label>
    <p class="inputName"> {{ inputName }}</p>
    <input 
      :placeholder="placeholder"
      type="text"
      :name="name"
      :required="required"
    />
  </label>
</template> 

<script>
export default {
  props: ['placeholder', 'name', 'inputName']
}
</script>