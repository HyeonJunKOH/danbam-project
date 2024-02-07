<template>
    <div id="main">
        <div v-scroll:#main="handleScroll">
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
            scrollPostion : 0
        }
    },
    methods:{
        handleScroll(e){
            this.scrollPostion = e.target.scrollTop;

            if(this.scrollPostion > 100){
                console.log("UP")
            } else {
                console.log("DOWN")
            }
        }
    }
}
</script>
<style scoped>
</style>