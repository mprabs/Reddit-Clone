<template>
  <div id="app">
    <Header @gotohome="page = 'Home'" />
    <div v-if="page == 'Home'" class="home__body">
      <div class="body__left">
        <CreatePost @change="page = 'Submit'" />
        <FilterTags :tags="tags" />
        <Posts />
        <Posts />
      </div>
      <div class="body__right">
        <TopGrowingCard />
        <Ads />
      </div>
    </div>
    <div v-else-if="page == 'Submit'">
      <SubmitPost />
    </div>
  </div>
</template>

<script>
import states from "./assets/data.json";
import Header from "./components/header"
import CreatePost from "./components/postCard"
import FilterTags from "./components/filterTags"
import Posts from "./components/posts"
import TopGrowingCard from "./components/topGrowing"
import Ads from "./components/ad"
import SubmitPost from "./components/submitPost/submitPost"
export default {
  name: "App",
  data() {
    return {
      page: "Home"
    }
  },
  computed: {
    tags() {
      return states.tags.map((item) => {
        return item;
      })
    }
  },
  components: {
    Header,
    CreatePost,
    FilterTags,
    Posts,
    TopGrowingCard,
    Ads,
    SubmitPost
  }
};
</script>

<style>
@import './assets/css/app.css';
#app {
  font-family:Verdana, Arial, Helvetica, sans-serif ;
}


</style>
