<template>
    <div id="section1">
        <left-nav/>
        <right-nav/>
        <plant-content/>
    </div>
</template>


<script>
import LeftNav from './LeftNav.vue'
import PlantContent from './PlantContent.vue'
import RightNav from './RightNav.vue'
export default {
    name:'section1',
    components:{
        LeftNav,
        PlantContent,
        RightNav
    }
}
</script>

<style>
#section1{
    width: 1170px;
    margin: 0 auto;
    margin-top: 70px;
    /* height: 100px; */
    /* background-color: aqua; */
}
</style>