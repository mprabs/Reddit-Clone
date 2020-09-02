<template>
  <div class="post__rules">
      <div class="rules__head">
          <img src="../../../assets/img/profile-avatar.png" alt="">
          <span>Posting to Reddit</span>
      </div>
      <div class="rules">
          <span>1. Remember the human</span>
          <span>2. Behave like you would in real life</span>
          <span>3. Look for the original source of content</span>
          <span>4. Search for duplicates before posting</span>
          <span>5. Read the community’s rules</span>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
    .post__rules {
        display: flex;
        background-color: white;
        border-radius: 5px;
        flex-direction: column;
    }

    .post__rules .rules__head {
        display: flex;
        align-items: center;
        padding: 15px 10px;
    }

    .rules__head img {
        height: 30px;
        border-radius: 15px;
        margin-right: 10px;
    }

    .rules__head span {
        font-size: 14px;
        font-weight: bold;
        opacity: 0.8;
    }

    .post__rules .rules {
        display: flex;
        flex-direction: column;
        justify-content: center;
        border-top: 1px solid rgb(221, 217, 217);
    }

    .post__rules .rules span {
        line-height: 40px;
        font-size: 13px;
        opacity: 0.8;
        padding-left: 10px;
        border-bottom: 1px solid rgb(216, 213, 213);
        border-width: 50%;
}
</style>