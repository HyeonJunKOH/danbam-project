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
                        <span class="login">로그인</span>
                    </a>
                </div>
                <div class="head_menu">
                    <ul>
                        <li class="menu" @mouseover="showMenu(1)" @mouseleave="hideMenu()">
                            <a href="">단밤 스토리</a>
                            <div class="menu_list" v-show="showMenuList === 1">
                                <ul>
                                    <li class="list">
                                        <a href="">브랜드</a>
                                    </li>
                                    <li class="list">
                                        <a href="">오시는 길</a>
                                    </li>
                                </ul>
                            </div>
                        </li>
                        <li class="menu" @mouseover="showMenu(2)" @mouseleave="hideMenu()">
                            <a href="">메뉴 소개</a>
                            <div class="menu_list1" v-show="showMenuList === 2">
                                <ul>
                                    <li class="list">
                                        <a href="">음료</a>
                                    </li>
                                    <li class="list">
                                        <a href="">푸드</a>
                                    </li>
                                </ul>
                            </div>
                        </li>
                        <li @mouseover="showMenu(3)" @mouseleave="hideMenu()">
                            <a href="">메뉴 주문</a>
                            <div class="menu_list2" v-show="showMenuList === 3">
                                <ul>
                                    <li class="list">
                                        <a href="">장바구니</a>
                                    </li>
                                    <li class="list">
                                        <a href="">주문내역</a>
                                    </li>
                                </ul>
                            </div>
                        </li>
                        <li @mouseover="showMenu(4)" @mouseleave="hideMenu()">
                            <a href="">매장</a>
                            <div class="menu_list3" v-show="showMenuList === 4">
                                <ul>
                                    <li class="list">
                                        <a href="">매장 찾기</a>
                                    </li>
                                </ul>
                            </div>
                        </li>
                        <li @mouseover="showMenu(5)" @mouseleave="hideMenu()">
                            <a href="">단밤 소식</a>
                            <div class="menu_list4" v-show="showMenuList === 5">
                                <ul>
                                    <li class="list">
                                        <a href="">공지사항</a>
                                    </li>
                                    <li class="list">
                                        <a href="">이벤트</a>
                                    </li>
                                    <li class="list">
                                        <a href="">FAQ</a>
                                    </li>
                                    <li class="list">
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
        data(){
            return{
                showMenuList: 0,
                isUnderlined:false
            }
        },
        methods:{
            showMenu(menuIndex){
                this.showMenuList = menuIndex

            },
            hideMenu(){
                this.showMenuList = 0;
            }
        }
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
/* 전체 위치 고정 */
.wrap{
    width: 100%;
    position: relative;
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
    background-color: #fff;
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
/* 전체 ul 스타일 지정 */
ul{
    list-style: none;
    padding: 0px;
    margin: 0px;
}
/* 상단 메뉴바 */
.head_menu{
    width: 100%;
    padding: 0, 300px;
}
.head_menu>ul{
    display: flex;
    justify-content: space-between;
}
.head_menu>ul>li{
    display: table-cell;
    font-weight: 550;
    flex: 1;
}
.head_menu>ul>li:hover{
    background-color:#FFC314;
    width: 50%;
}
/* 상단 메뉴바 백그라운드 컬러 지정 */


/* 하위 메뉴 리스트  */
.menu_list,.menu_list1,.menu_list2,.menu_list3,.menu_list4{
    padding: 20px;
}
.list{
    padding-bottom: 10px;
}
/* 하위 메뉴 리스트 underline 스타일 지정 시작 */
.list > a{
    display: inline-block;
    position: relative;
}
.list > a::after{
    content:"";
    position: absolute;
    left: 50%;
    bottom: 0;
    width: 0;
    height: 1px;
    background-color: black;
    transition: all .3s;
}
.list > a::before{
    content:"";
    position: absolute;
    right: 50%;
    bottom: 0;
    width: 0;
    height: 1px;
    background-color: black;
    transition: all .3s;
}
.list > a:hover::after{
    width: 50%;
}
.list > a:hover::before{
    width: 50%;
}
/* 하위 메뉴 리스트 underline 스타일 지정 끝 */
</style>