<template>
  <div class="filter__tags">
      <div class="tag__items">
        <div class="tag__item  tag__item__active">
            <i class="fas fa-rocket"></i>
            <span> Best</span>
        </div>
        <div class="tag__item">
            <i class="fas fa-burn"></i>
            <span> Hot</span>
        </div>
        <div class="tag__item">
            <i class="fas fa-certificate"></i>
            <span> New</span>
        </div>
        <div class="tag__item">
            <i class="fas fa-chart-bar"></i>
            <span> Top</span>
        </div>
        <div class="tag__item">
            <i class="fas fa-chart-line"></i>
            <span> Rising</span>
        </div>
      </div>
    <div class="filter__right__tags">
        <i class="fas fa-bars"></i>
        <i class="fas fa-sort-down"></i>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
    .filter__tags {
        margin-top: 20px;
        height: 5vh;
        background-color: white;
        display: flex;
        padding: 2vh;
        border-radius: 5px;
        justify-content: space-between;
    }

    .tag__items {
        display: flex;
        flex: 0.7;
        align-items: center;
        justify-content: space-evenly;
        font-size: 13px;
    }

    .filter__right__tags {
        flex: 0.3;
        display: flex;
        align-items: center;
        justify-content: flex-end;
    }

    .tag__item {
        padding: 8px 10px;
        font-weight: 900;
        opacity: 0.6;
    }

    .tag__item:hover {
        opacity: 1;
        cursor: pointer;
        border-radius: 20px;
        background: #f8f8f8;
    }

    .tag__item__active {
        border-radius: 20px;
        color: #0079D3;
        opacity: 1;
        background: #f8f8f8;
    }


    .filter__right__tags i {
        margin: 0 5px;
        color: #0079D3;
    }
</style>