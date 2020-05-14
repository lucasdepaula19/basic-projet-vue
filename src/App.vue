<template>
  <div id="app">
    <div class="container_1">
      <Header />
      <Menu />
    </div>
    <div class="container_2">
      <div class="Article">
        <Article
          v-for="article in articles"
          v-bind:key="article"
          :msg="article"
        />
      </div>
      <Sidebar />
    </div>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Menu from "./components/Menu.vue";
import Sidebar from "./components/Sidebar.vue";
import Article from "./components/Article.vue";

export default {
  name: "App",
  data() {
    return {
      articles: [
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus eu ligula non neque iaculis varius. Fusce eu nunc lorem. In nec sem sed justo fringilla aliquet non accumsan ex. In diam eros, faucibus vehicula maximus sit amet, ultrices lacinia libero. Sed scelerisque metus vitae neque semper, eget dictum odio scelerisque.",
        "Aliquam pharetra sit amet diam volutpat vulputate. Pellentesque gravida quam sed erat interdum hendrerit. Phasellus convallis volutpat posuere. Sed ac ornare ex. Etiam interdum efficitur mollis. In sit amet gravida nibh.",
        "Cras congue est quis ipsum ullamcorper feugiat. Quisque ac elit in dui pellentesque facilisis. In tristique efficitur posuere. Quisque sit amet mauris feugiat, sodales eros eu, pellentesque lorem. Aenean non lectus ac metus dignissim ullamcorper. Vivamus eget ex nisl. Nulla bibendum fringilla vehicula. Duis dui nulla, bibendum non ex eu, cursus tempus dui.",
        "ulla sed consectetur elit, ac auctor tortor. Pellentesque in eleifend nunc. In cursus, dolor a vulputate commodo, elit dui venenatis mi, vitae ornare erat leo eget quam. Etiam faucibus dui sed purus ultricies, ac pretium est vulputate. Phasellus tempus euismod urna, sit amet pellentesque nisl dictum a. Nulla facilisi. Sed eu odio sed erat condimentum ultricies sed laoreet purus. Proin accumsan arcu lorem, non mollis turpis luctus at. Nam iaculis nulla at lorem aliquet, in venenatis eros accumsan."
      ]
    };
  },
  components: {
    Header,
    Menu,
    Article,
    Sidebar
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #424e5a;
}

.container_1 {
  display: flex;
  flex-direction: column;
  margin: 5px;
}

.container_2 {
  display: flex;
  flex-direction: row;
  margin: 5px;
}

.Article {
  border: 1px solid;
  border-color: black;
  margin: 5px;
  padding: 1em;
  max-width: 80%;
}
</style>
