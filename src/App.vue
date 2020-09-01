<template>
  <div id="app">
    <Header />
    <div class="body">
      <div class="body__left">
        <SubmitPost />
        <FilterTags />
        <Posts />
        <Posts />
      </div>
      <div class="body__right">
        <TopGrowingCard />
        <Ads />
      </div>
    </div>
  </div>
</template>

<script>
import Header from "./components/header"
import SubmitPost from "./components/postCard"
import FilterTags from "./components/filterTags"
import Posts from "./components/posts"
import TopGrowingCard from "./components/topGrowing"
import Ads from "./components/ad"
export default {
  name: "App",
  components: {
    Header,
    SubmitPost,
    FilterTags,
    Posts,
    TopGrowingCard,
    Ads
  }
};
</script>

<style>
@import './assets/css/app.css';
#app {
  font-family:Verdana, Arial, Helvetica, sans-serif ;
}


</style>
