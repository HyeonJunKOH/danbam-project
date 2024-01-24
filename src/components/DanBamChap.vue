<template>
    <div class="chap_wrap">
        <ul>
            <li>MAIN</li>
            <li>MENU</li>
            <li>DANBAM</li>
            <li>EVENT</li>
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
.chap_wrap li {
    margin-bottom: 20px;
    cursor: pointer;
}
ul{
    list-style: none;
    padding: 0;
    margin: 0;
}
</style>