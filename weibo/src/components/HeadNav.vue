<template>
    <div id="headNav">
        <div class="headNav1">
            <h1 class="fl"><a href="#">新浪微博</a></h1>
            <div class="nav fr">
                <ul>
                    <li><a href="#"><span class="iconfont">&#xe60d;</span> 首页</a></li>
                    <li><a href="#"><span class="iconfont">&#xe63b;</span> 视频</a></li>
                    <li><a href="#"><span class="iconfont">&#xe726;</span> 发现</a></li>
                    <li><a href="#"><span class="iconfont">&#xe6a2;</span> 游戏</a></li>
                    <li><a href="#">注册</a></li>
                    <li style="margin-left: 10px;">|</li>
                    <li style="margin-left: 10px;"><a href="#">登录</a></li>
                </ul>
            </div>
            <div class="kuang fl" @click=getClick>
                <input style="text" id="inputSoSuo" :placeholder=msg+res[1].title>
                <span class="iconfont"><a href="#">&#xe69d;</a></span>
                <!-- 隐藏部分 -->
                <div class="searchHide">   
                    <div class="reso">
                        查看完整的热搜榜>>
                    </div>
                    <ul>
                        <li><a href="#"><i></i><span style="background-color: red;">1</span> {{ res[1].title }}</a></li>
                        <li><a href="#"><span style="background-color: #ff8140;">2</span> {{ res[2].title }}</a></li>
                        <li><a href="#"><span>3</span> {{ res[3].title }}</a></li>
                        <li><a href="#"><span>4</span> {{ res[4].title }}</a></li>
                        <li><a href="#"><span>5</span> {{ res[5].title }}</a></li>
                        <li><a href="#"><span>6</span> {{ res[6].title }}</a></li>
                        <li><a href="#"><span>7</span> {{ res[7].title }}</a></li>
                        <li><a href="#"><span>8</span> {{ res[8].title }}</a></li>
                        <li><a href="#"><span>9</span> {{ res[9].title }}</a></li>
                        <li><a href="#"><span>10</span> {{ res[10].title }}</a></li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>


<script>
import $ from 'jquery'
import remen from '@/./assets/remen.json'
export default {
    data(){
        return{
            res : [],
            msg:"大家正在搜："
        }
    },
    methods:{
        // 输入框的点击事件
        getClick:function (){
            $(".searchHide").css("display","block")
            $("#inputSoSuo").attr("placeholder",this.res[1].title)
        }
    },
    created(){
        this.res = remen;
        // document点击事件，用于隐藏，隐藏部分内容。
        document.addEventListener("click",function(event){
            let even = event || window.event,
                tag = even.target || even.srcElement;
            if(tag.id != "inputSoSuo")
            {
                document.getElementsByClassName("searchHide")[0].style.display = "none";
                $("#inputSoSuo").attr("placeholder","大家正在搜：" + remen[1].title);
            }
        },false)
        // 滚动出现盒子下面的阴影
        $(document).scroll(function(){
            let res = $(this).scrollTop();
            if(res >= 5){
                $("#headNav").css("box-shadow","0px 2px 3px #888888")
            }else{
                $("#headNav").css("box-shadow","none")
            }
        })
    }
}
</script>


<style>
@charset "utf-8";
@import '../assets/css/headNav.css';
#headNav{
    position: fixed;
    z-index: 999999999999999999999;
    top: 0px;
    left: 0px;
    width: 100%;
    height: 50px;
    /* background-color: aqua; */
    border-bottom: 1px solid #efefef;
    border-top: 2px solid #ff8140;
    background-color: rgba(255,255,255,.9);
}
#headNav .headNav1{
    width: 1280px;
    height: 48px;
    margin: 0 auto;
}
/* 左边logo */
#headNav .headNav1 h1 a{
    display: block;
    width: 140px;
    height: 48px;
    text-indent: -9999px;
    background-image: url(../assets/image/logo.jpg);
    overflow: hidden;
}
/* 右边导航 */
#headNav .headNav1 .nav ul li{
    float: left;
    list-style: none;
    height: 48px;
    line-height: 48px;
    text-align: center;
    margin-left: 25px;
}
#headNav .headNav1 .nav ul li a{
    font-size: 16px;
}
#headNav .headNav1 .nav ul li a span{
    font-weight: bold;
    font-size: 20px;
}
#headNav .headNav1 .nav ul li a:hover,#headNav .headNav1 .nav ul li a:hover span{
    color: #ff8140;
}
/* 中间搜索框 */
#headNav .headNav1 .kuang{
    width: 466px;
    height: 48px;
    margin-top: 10px;
    position: relative;
}
#headNav .headNav1 .kuang input{
    height: 28px;
    width: 466px;
}
#headNav .headNav1 .kuang .iconfont a{
    font-weight: bold;
    font-size: 22px;
    position: absolute;
    left: 430px;
    top:3px
}
#headNav .headNav1 .kuang span a:hover{
    cursor: pointer;
    color: #ff8140;
}
/* 中间搜索框隐藏部分 */
#headNav .headNav1 .kuang .searchHide{
    box-sizing: border-box;
    width: 470px;
    height: 335px;
    background-color: #fff;
    border: 1px solid #efefef;
    margin-top: 2px;
    padding: 1px;
    display: none;
    position: relative;
    z-index: 99999999;
}
#headNav .headNav1 .kuang .searchHide .reso{
    width: 465px;
    height: 30px;
    line-height: 30px;
    /* padding: 1px; */
    padding-left: 15px;
    margin-left: 1px;
    box-sizing: border-box;
    color: #ff8140; 
}
#headNav .headNav1 .kuang .searchHide .reso:hover{
    cursor: pointer;
    background-color: #efefef;
}
#headNav .headNav1 .kuang .searchHide ul li{
    list-style: none;
    box-sizing: border-box;
    width: 465px;
    height: 30px;
    padding: 1px;
    padding-right: 1px;
    line-height: 30px;
    /* padding-left: 15px; */
}
#headNav .headNav1 .kuang .searchHide ul li a{
    display: block;
    width: 465px;
    height: 30px;
}
#headNav .headNav1 .kuang .searchHide ul li a span{
    display: inline-block;
    margin-left: 15px;
    color: #fff;
    line-height: 15px;
    text-align: center;
    font-weight:bold;
    background-color: #9c9c9c;
    width: 15px;
    height: 15px;
    border-radius: 50%;
}
#headNav .headNav1 .kuang .searchHide ul li:hover a{
    cursor: pointer;
    color: #ff8140;
    background-color: #efefef;
}
</style>