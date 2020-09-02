<template>
    <div class="post__box">
        <div class="post__head">
            <div class="item">
                <i class="fas fa-comment-alt"></i>
                <span>Post</span>
            </div>
            <div class="item">
                <i class="fas fa-image"></i>
                <span>Images & Video</span>
            </div>
            <div class="item">
                <i class="fas fa-link"></i>
                <span>Link</span>
            </div>
            <div class="item">
                <i class="fas fa-list-ol"></i>
                <span>Poll</span>
            </div>
        </div>
        <div class="post__body">
            <input type="text" placeholder="Title">
            <textarea placeholder="Text(optional)" id="" cols="25" rows="10"></textarea>
        </div>
        <div class="post__tags">
            <div class="left__tags">
                <div class="item">
                    <i class="fas fa-plus"></i>
                    <span>OC</span>
                </div>
                <div class="item">
                    <i class="fas fa-plus"></i>
                    <span>SPOILER</span>
                </div>
                <div class="item">
                    <i class="fas fa-plus"></i>
                    <span>NSFW</span>
                </div>
                <div class="item">
                    <i class="fas fa-tag"></i>
                    <span>FLAIR</span>
                </div>
            </div>
            <div class="buttons">
                <button class="cancel">Cancel</button>
                <button class="done">POST</button>
            </div>
        </div>
        <div class="post__footer">
            <div class="reply">
                <input type="checkbox" checked>
                <span>Send me post reply notifications</span>
            </div>
            <span class="link">Connect accounts to share your post <i class="fas fa-info-circle"></i></span>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style>

.post__box {
    margin-top: 10px;
    background-color: white;
    border-radius: 10px;
    width: 100%;
}

.post__box .post__head {
    display: flex;
    justify-content: space-around;
    height: 50px;
}

.post__box .post__head .item {
    flex: 0.25;
    height: 100%;
    border-right: 1px solid rgb(218, 215, 215);
    border-bottom: 1px solid rgb(221, 218, 218);
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 13px;
    font-weight: bold;
    opacity: 0.5;
}

.post__box .post__head .item:hover {
    background-color: #F2F8FD;
    cursor: pointer;
}

.post__box .post__head .item i {
    margin-right: 5px;
}

.post__body {
    display: flex;
    margin-top: 10px;
    flex-direction: column;
    align-items: center;
}

.post__body input {
    width: 95%;
    height: 30px;
    padding-left: 10px;
    border: 1px solid rgb(223, 222, 222);
    border-radius: 5px;
}

.post__body textarea {
    margin-top: 10px;
    width: 94%;
    font-family: inherit;
    font-size: 12px;
    padding: 10px;
    border: 1px solid rgb(223, 222, 222);
}

.post__tags {
    display: flex;
    margin: 10px 10px;
    justify-content: space-between;
}

.post__tags .left__tags {
    display: flex;
    flex: 0.5;
    justify-content: space-around;
}

.post__tags .left__tags .item {
    border: 1px solid rgb(211, 209, 209);
    padding: 5px;
    opacity: 0.7;
    font-size: 12px;
    font-weight: bold;
}

.post__tags .left__tags .item i {
    margin-right: 5px;
}

.post__tags .buttons .cancel {
    border: 1px solid #0079D3;
    padding: 8px  15px;
    margin-right: 5px;
    border-radius: 5px;
    text-transform: uppercase;
    font-weight: bold;
    color: #0079D3;
    font-size: 12px;
    background-color: white;
}

.post__tags .buttons .done {
    background-color: #0079D3;
    color: white;
    padding: 9px 10px;
    border-radius: 5px;
    text-transform: uppercase;
    font-weight: bold;
    font-size: 12px;
    border: none;
}

.post__footer {
    margin-top: 20px;
    padding-left: 20px;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    background-color: #F6F7F8;
    height: 80px;
}

.post__footer .reply span {
    font-size: 12px;
    font-weight: 550;
    color: rgb(102, 99, 99);
    cursor: pointer;
}

.post__footer .reply input {
    padding: 10px;
    border-radius: 5px;
    background-color: #0079D3;
}

.post__footer > .link {
    font-weight: bold;
    color: #0079D3;
}

.post__footer .link:hover {
    cursor: pointer;
    text-decoration: underline;
}

.post__footer .link i {
    color: rgb(107, 103, 103);
}

input[type=checkbox] {
    transform: scale(1.2);
    margin-right: 10px;
    color: #0079D3;
}
</style>