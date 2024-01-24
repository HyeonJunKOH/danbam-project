<template>
    <div class="background_wrap">
        <img class="main_img" src="@/assets/mainpage.jpg">
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
    .background_wrap{
        width: 100%;
        height: auto;
        display: block;
        position: relative;
        z-index: 1;
    }
    .main_img{
        max-width: 100%; /* 이미지가 부모 요소를 초과하지 않도록 합니다. */
        height: auto; /* 이미지 비율을 유지하도록 합니다. */
    }
</style>