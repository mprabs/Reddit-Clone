<template>
    <div class="post__card">
        <img src="../assets/img/profile-avatar.png" alt="">
        <input @click="$emit('change')" type="text" placeholder="Create Post">
        <i class="fas fa-image"></i>
        <i class="fas fa-link"></i>
    </div>
</template>

<script>
export default {

}
</script>

<style>
.post__card {
    height: 5vh;
    background-color: white;
    display: flex;
    align-items: center;
    border: 1px solid #d3d1d1;
    padding: 2vh;
    border-radius: 5px;
    overflow: hidden;
}

.post__card input {
    flex: 1;
    min-width: 30px;
    padding: 0 10px;
    height: 6vh;
    border: 1px solid #abacad;
    border-radius: 5px;
    margin: 10px;
    background-color: #f8f8f8;
}

.post__card i {
    font-size: 22px;
    height: 4vh;
    width: 4vh;
    color: #abacad;
    padding: 1vh;
}

.post__card i:hover {
    background-color: #e0e0e2;
}

.post__card img {
    height: 40px;
    width: 40px;
    border-radius: 20px;
}


</style>