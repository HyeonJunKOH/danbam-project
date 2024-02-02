<template>
    <div class="chap_wrap">
        <ul>
            <li class="chap_list">
                <span></span>
                <div class="chap_list_title">MAIN</div>
            </li>
            <li class="chap_list">
                <span></span>
                <div class="chap_list_title">MENU</div>
            </li>
            <li class="chap_list">
                <span></span>
                <div class="chap_list_title">DANBAM</div>
            </li>
            <li class="chap_list">
                <span></span>
                <div class="chap_list_title">EVENT</div>
            </li>
        </ul>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
.chap_wrap{
    display: block;
    position: fixed;
    bottom: 0;
    left: 0;
    padding: 30px;
    text-align: left;
    z-index: 1;
    font-weight: 900;
}
.chap_wrap>ul{
    position: relative;
}
.chap_list{
    margin-bottom: 20px;
    cursor: pointer;
}
.chap_list span{
    width: 10px;
    background-color: black;
    opacity: 1;
    height: 2px;
    border-radius: 100%;
    cursor: pointer;
    display: inline-block;
    vertical-align: middle;
}
.chap_list_title{
    display: inline-block;
    padding-left: 0px;
    opacity: 1;
    vertical-align: middle;
    cursor: pointer;
}
ul{
    list-style: none;
    padding: 0;
    margin: 0;
}
</style>