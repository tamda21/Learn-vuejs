<template>

   <footer>
     <p>{{copyright}}</p>
   </footer>
  
  
</template>

<script>

export default {
  
  data () {
    return {
      copyright:'Copyright 2022 Vue Jokers'
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
