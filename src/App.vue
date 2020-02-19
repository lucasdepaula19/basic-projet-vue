<template>
  <div id="app">
    <Header/>
    <Menu/>
    <Sidebar/>
    <Article v-for="article in articles" v-bind:key="article"
    
    :msg="article"

     />
  </div>
</template>

<script>
  import Header from './components/Header.vue'
  import Menu from './components/Menu.vue'
  import Sidebar from './components/Sidebar.vue'
  import Article from './components/Article.vue'

  export default {
    name: 'App',
    data() {
      return {
        articles:[
          "texto de teste no componente article 1",
          "texto de teste no componente article 2",
          "texto de teste no componente article 3"
        ]
      }
    },
    components: {
      Header,
      Menu,
      Sidebar,
      Article
    }
  }
</script>

<style>
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
</style>
