<template>
  <h1>hello</h1>
  <ul id="example-1">
    <li v-for="item in items" :key="item.message">
      {{ item.message }}
    </li>
  </ul>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data(){
    return {
      items: [
        {message:'Tom'},
        {message:'Gianni'},
        {message:'Laetitia'},
        {message:'Sammy'},
        {message:'George Gaming'}
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
