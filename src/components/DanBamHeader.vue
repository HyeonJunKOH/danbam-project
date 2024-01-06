<template>
    <div class="wrap">
        <div class="head_wrap">
            <div class="head">
                <div class="head_logo">
                    <h1>DANBAM COFEE</h1>
                </div>
                <div class="head_login">
                    <span class="head_sign">회원가입</span>
                    <span>로그인</span>
                </div>
                <div class="head_menu">
                    <ul>
                        <li>단밤 스토리</li>
                        <li>메뉴 소개</li>
                        <li>메뉴 주문</li>
                        <li>매장</li>
                        <li>단밤 소식</li>
                    </ul>
                </div>
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
}
.head_wrap.head{
    width: 100%;
    max-width: 1280px;
    margin: 0, auto;
    position: relative;
    box-sizing: border-box;
    display: flex;
}
.head_login{
    position: absolute;
    right: 137px;
    top: 30px;
}
.head_sign{
    margin-right: 30px;
}
.head_menu{
    width: 100%;
    padding: 0, 300px;
}
.head_menu>ul{
    display: table;
    width: 100%;
}
ul{
    list-style: none;
    padding: 0px;
    margin: 0px;
}
.head_menu>ul>li{
    display: table-cell;
}
li{
    font-weight: 550;
}

</style>