<template>
  <div>
  <app-header v-bind:title="title"></app-header>
  <jokers v-bind:jokers="jokers"></jokers>
  <hr>
  <jokers v-bind:jokers="jokers"></jokers>
  <app-footer  v-bind:title="title"></app-footer>
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
       {name:'Loujaine',discrpt:'Child Of Family',show:false},
       {name:'ali',discrpt:'Grand Father',show:false}
       ],
       title:'Vue Jokers'
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
