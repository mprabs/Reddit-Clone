<template>
  <div class="ad">
      <i class="fas fa-shield-alt"></i>
      <div class="ad__details">
          <strong class="title">Reddit Premium</strong>
          <span>The best Reddit experience, with monthly Coins</span>
      </div>
      <div class="button">
          <button>TRY NOW</button>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
.ad {
    margin-top: 20px;
    height: 5vh;
    background-color: white;
    display: flex;
    padding: 2vh;
    border-radius: 5px;
    align-items: center;
    font-size: 11px;
}
.ad i {
    flex: 0.1;
    font-size: 20px;
    color: #FF4500;
}
.ad .ad__details {
    flex: 0.6;
    display: flex;
    flex-direction: column;
}

.ad .button {
    flex: 0.3;
}

.ad .button button {
    padding: 5px 10px;
    background-color: #FF4500;
    color: white;
    border: none;
    border-radius: 5px;
    font-weight: bold;
}
</style>