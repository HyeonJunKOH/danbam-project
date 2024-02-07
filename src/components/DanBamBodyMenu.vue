<template>
    <div>
        <div class="background_wrap">
            <img class="main_img" src="@/assets/mainpage.jpg">
        </div>

        <div v-show="!showImage">
            단밤커피 딸기 시즌 신메뉴
        </div>
        <div>
            <h2>
                <span>Heart Berry Attack!</span>
            </h2>
        </div>
    </div>
</template>
<script>
export default {
    data(){
        return{
            showImage: true
        };
    },
    mounted() {
        window.addEventListener('scroll',this.handleScroll);
    },
    beforeUnmount() {
        window.removeEventListener('scroll',this.handleScroll);
    },
    methods:{
        handleScroll(){
            // 여기에서 스크롤 위치에 따라 showImage 상태 업데이트
            // 예: 스크롤이 특정 위치 이상이면 showImage를 false로 업데이트
            // 아니면 true로 유지
            if(window.scrollY > 200){
                this.showImage = false;
            } else {
                this.showImage = true;
            }
        }
    }
}
</script>
<style scoped>
.background_wrap {
  width: 100%;
  height: auto;
  display: block;
  position: relative;
  z-index: 1;
}

.main_img {
  max-width: 100%;
  height: auto;
}
</style>