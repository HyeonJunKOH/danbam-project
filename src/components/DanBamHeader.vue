<template>
    <div class="wrap">
        <div class="head_wrap">
            <div class="head">
                <h1>DANBAM COFEE</h1>
                <span>단밤 스토리</span>
                <span>메뉴 소개</span>
                <span>메뉴 주문</span>
                <span>매장</span>
                <span>단밤 소식</span>
                <span>회원가입</span>
                <span>로그인</span>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
    div {
        display: block;
    }
    .wrap{
        width: 100%;
        position: relative; /* 상대 위치 지정 */
    }
    .head_wrap {
        position: fixed; 
        top: 0;
        margin: auto, 0;
        width: 100%;
        z-index: 9999; /* 사진보다 위에 위치하도록 설정 */
        vertical-align: middle;
        padding: 0px, 20px;
        text-align: center;
        display: flex; /* Flexbox 사용 */
        justify-content: space-between; /* 요소들 사이의 간격을 최대로 설정 */
        align-items: center;
    }
    .head_wrap.head{
        width: 100%;
        max-width: 1280px;
        margin: 0, auto;
        position: relative;
    }
    
</style>