<template>
  <div class="post">
      <div class="left__vote__icons">
            <i :class="`fas fa-arrow-alt-up ${ upVoted ? 'red' : '' }`" @click="increaseVoteCount()"></i>

            <span :class="`vote__count ${ upVoted ? 'red' : downVoted ? 'blue' : '' }`">
                {{ voteCount || VOTE_COUNT }}
            </span>

            <i :class="`fas fa-arrow-alt-down ${downVoted ? 'blue' : '' }`" @click="decreaseVoteCount()"></i>
      </div>
      <div class="post__content">
          <div class="post__head">
            <img src="../assets/img/profile-avatar.png" alt="">
            <span class="user__name"><strong>r/prabin</strong> </span>
            <div class="post__details">
               <p>• Posted by Prabin 3 hours ago</p> 
            </div>
          </div>
          <div class="post__body">
              <div class="post__title">
                  <strong>The Mumbai Indians recreation room looks like a great place to unwind <span class="badge"> Discussion </span> </strong>
              </div>
              <div class="post__image">
                  <img src="https://picsum.photos/200/300" alt="">
              </div>
          </div>
          <div class="post__footer">
              <div class="post__item">
                  <i class="fas fa-comment-alt"></i>
                  <span>24 comments</span>
              </div>
              <div class="post__item">
                  <i class="fas fa-gift"></i>
                  <span>Give Award</span>
              </div>
              <div class="post__item">
                  <i class="fas fa-share"></i>
                  <span>Share</span>
              </div>
              <div class="post__item">
                  <i class="fas fa-bookmark"></i>
                  <span>Save</span>
              </div>
              <div class="post__item">
                  <i class="fas fa-ellipsis-h"></i>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export const VOTE_COUNT = 15;
export default {
    data() {
        return {
            VOTE_COUNT,
            voteCount: "",
            upVoted: false,
            downVoted: false
        }
    },
    methods: {
        increaseVoteCount() {
            if(this.upVoted) {
                this.voteCount = ""
                return;
            }
            this.voteCount = VOTE_COUNT + 1;
        },
        decreaseVoteCount() {
            if(this.downVoted) {
                this.voteCount = ""
                return;
            }
            this.voteCount = VOTE_COUNT - 1;
        }
     },
     watch: {
         voteCount() {
             if(this.voteCount == this.VOTE_COUNT - 1) {
                 this.upVoted = false
                 this.downVoted = true
             } else if (this.voteCount == this.VOTE_COUNT + 1) {
                 this.downVoted = false
                 this.upVoted = true
             } else {
                 this.downVoted = this.upVoted = false
             }
         },
     }
}
</script>

<style>
.post {
    margin-top: 20px;
    height: auto;
    background-color: white;
    display: flex;
    border-radius: 5px;
    padding: 1px;
    width: 100%;
    overflow-y: scroll;
    border: 1px solid #d3d1d1;
}

.post:hover {
    border: 1px solid rgb(153, 152, 152);
}

.left__vote__icons {
    width: 20px;
    display: flex;
    flex-direction: column;
    background-color: #F8F9FA;
    padding: 10px;
}

.left__vote__icons i {
    font-size: 15px;
    opacity: 0.6;
    font-weight: bolder;
}

.left__vote__icons span {
    margin: 5px 0;
    font-size: 12px;
    font-weight: bold;
}

.red {
    color: red;
}

.blue {
    color: blue;
}

.post__content {
    padding: 5px 10px;
    display: flex;
    flex-direction: column;
    margin-bottom: 10px;
}

.post__head {
    display: flex;
    align-items: center;
    height: 30px;
    font-size: 12px;
}

.post__head .user__name {
    margin: 0 10px;
    opacity: 1;
}

.post__head .post__details {
    opacity: 0.7;
}

.post__content .post__head img {
    height: 20px;
    border-radius: 10px;
    object-fit: contain;
}

.post__body .post__title .badge {
    padding: 3px 10px;
    background-color: red;
    font-size: 10px;
    color: white;
    border-radius: 30px;
}

.post__body .post__title {
    display: flex;
    align-items: center;
}

.post__image {
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 10px 0;
}


.post__footer {
    display: flex;
    color: #7e8081;
    font-size: 12px;
    justify-content: flex-start;
}

.post__item {
    margin: 0 5px;
    display: flex;
    align-items: center;
    font-weight: bold;
}
.post__item i {
    margin-right: 5px;
}

.fa-arrow-alt-up, .fa-arrow-alt-down {
    cursor: pointer;
    font-weight: bold;
}

::-webkit-scrollbar {
    width: 0px;  /* Remove scrollbar space */
    background: transparent;  /* Optional: just make scrollbar invisible */
    height: 10px;
}

::-webkit-scrollbar-thumb {
    background: #909499;
}

</style>