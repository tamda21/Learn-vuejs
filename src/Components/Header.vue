<template>
  
   <header>
     <h1 v-on:click="changeTitle">{{title}}</h1>
   </header>
  
  
</template>

<script>

export default {
  props:{
    title:{
      type:String
    }
  },
  data () {
    return {
      //title:'Vue Jokers'
    }
  },
  methods:{
    changeTitle:function () {
     // this.title='Vue'
     this.$emit('titleChange','Vu')
    }
  }
}
</script>

<style scoped>
 header{
   background-color: lightgreen;
   padding: 10px;
 }
 h1{
   color: #222;
   text-align: center;
   font-family: Arial;
 }
</style>
