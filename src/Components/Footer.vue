<template>

   <footer>
     <p>{{copyright}} {{title}}</p>
   </footer>
  
  
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
      copyright:'Copyright 2022'
    }
  },
  methods:{
    
  }
}
</script>

<style scoped>
 footer{
   background-color: #222;
   padding: 6px;
 }
 p{
   color: lightgreen;
   text-align: center;
 }
</style>
