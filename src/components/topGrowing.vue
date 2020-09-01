<template>
  <div class="top__growing">
      <div class="top__growing__header">
          <img src="https://picsum.photos/200/300" alt="">
          <span>Today's top growing communities</span>
      </div>
      <div class="top__growing__body">
          <div class="top__growing__item">
              <span>1</span>
              <i class="fas fa-sort-up"></i>
              <img src="../assets/img/profile-avatar.png" alt="">
              <span class="top__growing__user">r/prabinAcharya</span>
          </div>
          <div class="top__growing__item">
              <span>2</span>
              <i class="fas fa-sort-up"></i>
              <img src="../assets/img/profile-avatar.png" alt="">
              <span class="top__growing__user">r/prabinAcharya</span>
          </div>
          <div class="top__growing__item">
              <span>3</span>
              <i class="fas fa-sort-down"></i>
              <img src="../assets/img/profile-avatar.png" alt="">
              <span class="top__growing__user">r/prabinAcharya</span>
          </div>
          <div class="top__growing__item">
              <span>4</span>
              <i class="fas fa-sort-down"></i>
              <img src="../assets/img/profile-avatar.png" alt="">
              <span class="top__growing__user">r/prabinAcharya</span>
          </div>
          <div class="top__growing__item">
              <span>5</span>
              <i class="fas fa-sort-down"></i>
              <img src="../assets/img/profile-avatar.png" alt="">
              <span class="top__growing__user">r/prabinAcharya</span>
          </div>
          <div class="top__growing__button">
            <button>VIEW ALL</button>
          </div>
          <div class="top__growing__footer__tags">
              <div class="top__tag__item">Sports</div>
              <div class="top__tag__item">News</div>
              <div class="top__tag__item">Gaming</div>
              <div class="top__tag__item">Art</div>
          </div>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
.top__growing {
    background-color: white;
    display: flex;
    justify-content: space-between;
    flex-direction: column;
    border-radius: 5px;
}

.top__growing .top__growing__header {
    position: relative;
    height: 80px;
    overflow: hidden;
    width: 100%;
}

.top__growing__header img {
    position: absolute;
    top: 0;
    left: 0;
    min-width: 100%;
    border-radius: 5px;
}

.top__growing__header span {
    position: absolute;
    bottom: 10px;
    color: white;
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100%;
    z-index: 9999;
}

.top__growing__item {
    display: flex;
    justify-content: flex-start;
    padding-left: 10px;
    align-items: center;
    height: 50px;
    border-top: 1px solid rgb(228, 226, 226);
}

.top__growing__item img {
    height: 30px;
    border-radius: 15px;
    margin: 0 10px;
    opacity: 0.6;
}

.top__growing__item span {
    font-weight: bold;
    font-size: 13px;
    margin: 0 10px;
}

.top__growing__item .fa-sort-down {
    color: red;
}

.top__growing__item .fa-sort-up {
    color: greenyellow;
}

.top__growing__button {
    display: flex;
    align-items: center;
    justify-content: center;
}

.top__growing__button button {
    width: 90%;
    padding: 10px;
    background-color: #0079D3;
    color: white;
    border: none;
    border-radius: 5px;
    font-size: 12px;
}

.top__growing__footer__tags {
    display: flex;
    padding: 10px;
    justify-content: space-evenly;
    align-items: center;
    height: 50px;
}

.top__tag__item {
    font-size: 11px;
    color: #0079D3;
    background-color: rgb(245, 245, 245);
    padding: 8px;
    cursor: pointer;
}

.top__tag__item:hover {
    background-color: rgb(233, 233, 233);
}


</style>