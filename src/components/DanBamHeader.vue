<template>
    <div class="wrap">
        <div class="head_wrap">
            <div class="head">
                <div class="head_logo">
                    <h1>DANBAM COFEE</h1>
                </div>
                <div class="head_login">
                    <a href="">
                        <span class="head_sign">회원가입</span>
                    </a>
                    <a href="">
                        <span>로그인</span>
                    </a>
                </div>
                <div class="head_menu">
                    <ul>
                        <li>
                            <a href="">단밤 스토리</a>
                            <div>
                                <ul>
                                    <li>
                                        <a href="">브랜드</a>
                                    </li>
                                    <li>
                                        <a href="">오시는 길</a>
                                    </li>
                                </ul>
                            </div>
                        </li>
                        <li>
                            <a href="">메뉴 소개</a>
                            <div>
                                <ul>
                                    <li>
                                        <a href="">음료</a>
                                    </li>
                                    <li>
                                        <a href="">푸드</a>
                                    </li>
                                </ul>
                            </div>
                        </li>
                        <li>
                            <a href="">메뉴 주문</a>
                            <div>
                                <ul>
                                    <li>
                                        <a href="">장바구니</a>
                                    </li>
                                    <li>
                                        <a href="">주문내역</a>
                                    </li>
                                </ul>
                            </div>
                        </li>
                        <li>
                            <a href="">매장</a>
                            <div>
                                <ul>
                                    <li>
                                        <a href="">매장 찾기</a>
                                    </li>
                                </ul>
                            </div>
                        </li>
                        <li>
                            <a href="">단밤 소식</a>
                            <div>
                                <ul>
                                    <li>
                                        <a href="">공지사항</a>
                                    </li>
                                    <li>
                                        <a href="">이벤트</a>
                                    </li>
                                    <li>
                                        <a href="">FAQ</a>
                                    </li>
                                    <li>
                                        <a href="">고객의 소리</a>
                                    </li>
                                </ul>
                            </div>
                        </li>
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
a{
    text-decoration: none;
    color: black;
}
.wrap{
    width: 100%;
    position: relative; /* 상대 위치 지정 */
}
/* 상단 배너 */
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
/* 상단 배너 효과 */
.head_wrap:hover{
    background: #fff;
    box-shadow: 0px, 0px, 5px, 0px rgba(0, 0, 0, 0.1);
}
.head_wrap.head{
    width: 100%;
    max-width: 1280px;
    margin: 0, auto;
    position: relative;
    box-sizing: border-box;
    display: flex;
}
/* 회원가입 */
.head_login{
    position: absolute;
    right: 137px;
    top: 30px;
    font-weight: 550;
    cursor: pointer;
}
/* 로그인 */
.head_sign{
    margin-right: 30px;
}
/* 상단 메뉴바 */
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
    cursor: pointer;
    font-weight: 550;
}

</style>