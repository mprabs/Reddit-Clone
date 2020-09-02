<template>
  <div class="links__card">
    <div class="all__links">
        <div class="left">
            <span>Help</span>
            <span>Reddit App</span>
            <span>Reddit Coins</span>
            <span>Reddit Premium</span>
            <span>Reddit Gift</span>
        </div>
        <div class="right">
            <span>About</span>
            <span>Careers</span>
            <span>Press</span>
            <span>Advertise</span>
            <span>Blog</span>
            <span>Terms</span>
            <span>Content Policy</span>
            <span>Privacy Policy</span>
            <span>Mod Policy</span>
        </div>
    </div>      
    <span class="copy__right">Reddit Inc © 2020. All rights reserved</span>
  </div>
</template>

<script>
export default {

}
</script>

<style>
.links__card {
    margin-top: 10px;
    background-color: white;
    padding: 10px;
    font-size: 12px;
}

.links__card .all__links {
    display: flex;
    margin-bottom: 20px;
}

.all__links .left, .all__links .right {
    display: flex;
    flex: 0.5;
    line-height: 20px;
    flex-direction: column;
}

</style>