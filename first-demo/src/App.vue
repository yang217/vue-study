<template>
  <div id="app">
   <h1 @click="getshow">{{title}}</h1>
   <input v-model="title">
   <ul>
    <li v-for="name in fruits">
      {{name.name}}
    </li>
   </ul>
  
  </div>
</template>

<script>
export default {
  data:function(){
    return {
      title:'my name is yanghao',
      fruits:[
        {name:"apple"},
        {name:"banana"},
        {name:"tool"}
      ]
    
    }
  },
  methods:{
    getshow: function(){
      this.title=this.title+'xiamawen'
    }
  }
 
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
