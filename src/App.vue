<template>
  <ul>
    <li v-for="fruit in newFruits" 
    :key="fruit.id">
      {{ fruit.name }}
    </li>
  </ul>
</template>

<script>
export default {
  data() {
    return {
      fruits:['Apple','Banana','Cherry']
    }
  },
  computed: {
    newFruits() {
      return this.fruits.map((fruit, index)=>{
        return{
          id: index,
          name: fruit
        }
      })
    }
  }
}
</script>