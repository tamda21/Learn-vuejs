<template>
  <div id="jokers">
    <ul>
      <li v-for="joker in jokers" v-on:click="joker.show=!joker.show">
        <h2>{{joker.name}}</h2>
        <h3 v-show="joker.show">{{joker.discrpt}}</h3>
      </li>
    </ul>
    <button v-on:click="handelDelet">Delet</button>
  </div>
</template>

<script>

export default {
  props:{
    jokers:{
      type:Array
    }
  },
  data () {
    return {
     
    }
  },
  methods:{
handelDelet:function(){
      this.jokers.pop()
    }
  }
}
</script>

<style scoped>
 #jokers {
   max-width: 1200px;
   width: 100%;
   margin: 40px auto;
   padding: 0 20px;
   box-sizing: border-box;
 }
 ul{
   display: flex;
   flex-wrap: wrap;
   list-style: none;
   padding: 0;
 }
 li{
   flex-basis: 300px;
   flex-grow: 1;
   text-align: center;
   border: 1px solid #222;
   padding: 30px;
   margin: 10px;
 }
</style>
