<template>
  <div class="submit__post">
    <div class="left__body">
        <div class="top__header">
            <div class="title">Create a post</div>
            <div class="badge">Drafts <span> 0 </span></div>
        </div>
        <hr />
        <div class="select__community">
            <div class="left__side">
                <img src="../../assets/img/profile-avatar.png" alt="">
                <span>Choose a community</span>
            </div>
            <i class="fas fa-sort-down"></i>
        </div>
        <Markdown />
    </div>
    <div class="right__body">
        <RedditRules />
        <p class="text">Please be mindful of reddit's <span>content policy</span> and practice good <span>reddiquette</span>.</p>
        <LinksCard />
    </div>
  </div>
</template>

<script>
import Markdown from "./componentsInIt/markdown"
import RedditRules from "./componentsInIt/redditRules"
import LinksCard from "./componentsInIt/linksCard"
export default {
    components: {
        Markdown,
        RedditRules,
        LinksCard
    }
}
</script>

<style>
.submit__post {
    margin-top: 15vh;
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    flex-direction: row;
    justify-content: center;
    background-color: #DAE0E6;
}

.submit__post .left__body {
    flex: 0.6;
    display: flex;
    flex-direction: column;
}

.submit__post .right__body {
    flex: 0.23;
}

.submit__post .left__body .top__header {
    display: flex;
    justify-content: space-between;
}

.submit__post .top__header .badge {
    color: #0079D3;
    text-transform: uppercase;
    font-weight: bold;
    font-size: 12px;
}

.submit__post .top__header .badge span {
    padding: 2px 5px;
    background-color: rgb(128, 128, 131);
    color: white;
}

.submit__post .top__header .title {
    font-weight: bold;
    opacity: 0.8;
}

.submit__post .left__body hr {
    width: 100%;
    border-top: 1px solid white;
    margin-bottom: 15px;
}

.select__community {
    background-color: white;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 5px;
    width: 45%;
    border-radius: 3px;
}

.select__community .left__side {
    display: flex;
    align-items: center;
}

.select__community i {
    margin-right: 10px;
    height: 80%;
}

.select__community .left__side span {
    font-size: 12px;
    opacity: 0.8;
}

.select__community img{
    height: 30px;
    border-radius: 15px;
    margin-right: 10px;
}

.right__body .text {
    font-size: 11px;
    margin: 20px 0;
    color: rgb(133, 131, 130);
}

.right__body .text span {
    color: #0079D3;
    cursor: pointer;
}

@media screen and (max-width:1000px) {
    .submit__post {
        flex-direction: column;
        margin: 10px;
    }
}

</style>