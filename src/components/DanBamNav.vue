<template>
    <div class="nav_wrap">
        <div class="nav">
            <ul>
                <li>
                    <a href="">
                        <div class="table">고객센터</div>
                        <div class="table0">문의/접수</div>
                    </a>
                </li>
                <li>
                    <a href="">
                        <div class="table1">메뉴 주문</div>
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
    /* 네비바 전체 */
    .nav_wrap{
        position: fixed;
        right: 30px;
        top: 30%;
        text-align: center;
        font-size: 0.9rem;
        z-index: 3;
    }
    /* 네비바 스타일 */
    .nav > ul >li{
        list-style: none;
        background: #E6B36D;
        overflow: hidden;
        width: 110px;
        height: 110px;
        border-radius: 100%;
        box-shadow: 0px 5px 10px 0px rgba(0,0,0,0.3);
        margin-bottom: 15px;
    }
    .nav > ul >li > a{
        display: block;
        text-decoration: none;
        color: black;
        cursor: pointer;
    }
    /* 고객센터 */
    .table{
        margin-top: 30px;
        font-weight: 550;
    }
    .nav > ul > li:hover{
        background-color: #FFC314;
    }
    /* 문의접수 */
    .table0{
        font-weight: 550;
        font-size: 1.2rem;
    }
    /* 메뉴 주문 */
    .table1{
        margin-top: 40px;
        font-weight: 550;
        font-size: 1.2rem;
    }
</style>