<template>
    <div id="leftNav" @click=leftNavClick>
        <ul>
            <li><a href="#" class="hong">热门</a></li>
            <li><a href="#">头条</a></li>
            <li><a href="#">视频</a></li>
            <li><a href="#">榜单</a></li>
            <li><a href="#">搞笑</a></li>
            <li><a href="#">社会</a></li>
            <li><a href="#">时尚</a></li>
            <li><a href="#">电影</a></li>
            <li><a href="#">美女</a></li>
            <li><a href="#">体育</a></li>
            <li><a href="#">动漫</a></li>
        </ul>
    </div>
</template>


<script>
import $ from 'jquery'
export default {
    methods:{
        leftNavClick:function(event){
            let even = event || window.event,
                tag = even.target || even.srcElement;        
            $("#leftNav ul").children().children().removeClass("hong")
            $(tag).addClass("hong");
        }
    },
    mounted(){
        // 滚动悬浮左侧的导航栏
        $(document).scroll(function(){
            let res = $(this).scrollTop();
            if(res >= 10){
                $("#leftNav").css("position","fixed")
                $("#leftNav").css("top","54px")
                // $("#plantContent").css("margin-left","60px")
            }else{
                $("#leftNav").css("position","static")
                // $("#plantContent").css("margin-left","30px")
            }
        })
    }
}
</script>

<style>
#leftNav{
    width: 110px;
    height: 462px;
    float: left;
    background-color: #fff;
}
#leftNav ul li{
    border-radius: 5px;
    list-style: none;
    text-align: center;
    width: 110px;
    height: 40px;
    line-height: 40px;
    margin-top: 2px;
    color: #9c9c9c;
}
/* #leftNav ul li:hover{
    background-color: #fb3c31;
    color: #fff;
} */
#leftNav ul li a:hover{
    color: #fff;
    background-color: #fb3c31;
}
#leftNav ul li a{
    border-radius: 5px;
    display: inline-block;
    width: 110px;
    height: 40px;
    font-size: 18px;
    font-weight :500;
}
#leftNav ul li a.hong{
    color: #fff;
    background-color: #fb3c31;
}
</style>