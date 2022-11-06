<template>
  <div>
  <app-header></app-header>
  <jokers v-bind:jokers="jokers"></jokers>
  <app-footer></app-footer>
  </div>
</template>

<script>
import Header from './Components/Header';
import Footer from './Components/Footer';
import Jokers from './Components/Jokers';
export default {
  components:{
    'app-header':Header,
    'app-footer':Footer,
    'jokers':Jokers
  },
  data () {
    return {
      jokers:[
       {name:'Abde',discrpt:'Father Of Family',show:false},
       {name:'Meryem',discrpt:'Mother Of Family',show:false},
       {name:'Loujaine',discrpt:'Child Of Family',show:false}
       ]
    }
  },
  methods:{
    
  }
}
</script>

<style>
body{
  margin: 0;
  padding: 0;
}
</style>
