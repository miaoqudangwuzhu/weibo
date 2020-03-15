<template>
    <div id="plantContent">
        <!-- 轮播 -->
        <div id="daLunBo">
            <div class="daLunBo1 clearfix" style="transform: translateX(0px);">
                <!-- 1 -->
                <div class="lunbo">
                    <div class="imgLeft fl">
                        <a href="#">
                            <img :src="require('../'+resLunBo[1].imgSrc)">
                            <div class="leftText">
                                <h3>{{ resLunBo[1].title }}</h3>
                                <p>{{ discussArray[0] }}讨论  {{ readArray[0] }}阅读</p>
                            </div>
                        </a>
                    </div>
                    <div class="fr imgRight">
                        <img :src="require('../'+resLunBo[9].imgSrc)">
                        <img :src="require('../'+resLunBo[10].imgSrc)" style="margin-top:5px;">
                        <div class="text1">
                            <h3>#{{ resLunBo[9].title }}#</h3>
                        </div>
                        <div class="text2">
                            <h3>#{{ resLunBo[10].title }}#</h3>
                        </div>
                    </div>
                </div>
                <!-- 2 -->
                <div class="lunbo">
                    <div class="imgLeft fl">
                        <a href="#">
                            <img :src="require('../'+resLunBo[2].imgSrc)">
                            <div class="leftText">
                                <h3>{{ resLunBo[2].title }}</h3>
                                <p>{{ discussArray[1] }}讨论  {{ readArray[1] }}阅读</p>
                            </div>
                        </a>
                    </div>
                    <div class="fr imgRight">
                        <img :src="require('../'+resLunBo[11].imgSrc)">
                        <img :src="require('../'+resLunBo[12].imgSrc)" style="margin-top:5px;">
                        <div class="text1">
                            <h3>#{{ resLunBo[11].title }}#</h3>
                        </div>
                        <div class="text2">
                            <h3>#{{ resLunBo[12].title }}#</h3>
                        </div>
                    </div>
                </div>
                <!-- 3 -->
                <div class="lunbo">
                    <div class="imgLeft fl">
                        <a href="#">
                            <img :src="require('../'+resLunBo[3].imgSrc)">
                            <div class="leftText">
                                <h3>{{ resLunBo[3].title }}</h3>
                                <p>{{ discussArray[2] }}讨论  {{ readArray[2] }}阅读</p>
                            </div>
                        </a>
                    </div>
                    <div class="fr imgRight">
                        <img :src="require('../'+resLunBo[13].imgSrc)">
                        <img :src="require('../'+resLunBo[14].imgSrc)" style="margin-top:5px;">
                        <div class="text1">
                            <h3>#{{ resLunBo[13].title }}#</h3>
                        </div>
                        <div class="text2">
                            <h3>#{{ resLunBo[14].title }}#</h3>
                        </div>
                    </div>
                </div>
                <!-- 4 -->
                <div class="lunbo">
                    <div class="imgLeft fl">
                        <a href="#">
                            <img :src="require('../'+resLunBo[4].imgSrc)">
                            <div class="leftText">
                                <h3>{{ resLunBo[4].title }}</h3>
                                <p>{{ discussArray[3] }}讨论  {{ readArray[3] }}阅读</p>
                            </div>
                        </a>
                    </div>
                    <div class="fr imgRight">
                        <img :src="require('../'+resLunBo[15].imgSrc)">
                        <img :src="require('../'+resLunBo[16].imgSrc)" style="margin-top:5px;">
                        <div class="text1">
                            <h3>#{{ resLunBo[15].title }}#</h3>
                        </div>
                        <div class="text2">
                            <h3>#{{ resLunBo[16].title }}#</h3>
                        </div>
                    </div>
                </div>
                <!-- 5 -->
                <div class="lunbo">
                    <div class="imgLeft fl">
                        <a href="#">
                            <img :src="require('../'+resLunBo[5].imgSrc)">
                            <div class="leftText">
                                <h3>{{ resLunBo[5].title }}</h3>
                                <p>{{ discussArray[4] }}讨论  {{ readArray[4] }}阅读</p>
                            </div>
                        </a>
                    </div>
                    <div class="fr imgRight">
                        <img :src="require('../'+resLunBo[17].imgSrc)">
                        <img :src="require('../'+resLunBo[18].imgSrc)" style="margin-top:5px;">
                        <div class="text1">
                            <h3>#{{ resLunBo[17].title }}#</h3>
                        </div>
                        <div class="text2">
                            <h3>#{{ resLunBo[18].title }}#</h3>
                        </div>
                    </div>
                </div>
                <!-- 6 -->
                <div class="lunbo">
                    <div class="imgLeft fl">
                        <a href="#">
                            <img :src="require('../'+resLunBo[6].imgSrc)">
                            <div class="leftText">
                                <h3>{{ resLunBo[6].title }}</h3>
                                <p>{{ discussArray[5] }}讨论  {{ readArray[5] }}阅读</p>
                            </div>
                        </a>
                    </div>
                    <div class="fr imgRight">
                        <img :src="require('../'+resLunBo[19].imgSrc)">
                        <img :src="require('../'+resLunBo[20].imgSrc)" style="margin-top:5px;">
                        <div class="text1">
                            <h3>#{{ resLunBo[19].title }}#</h3>
                        </div>
                        <div class="text2">
                            <h3>#{{ resLunBo[20].title }}#</h3>
                        </div>
                    </div>
                </div>
                <!-- 7 -->
                <div class="lunbo">
                    <div class="imgLeft fl">
                        <a href="#">
                            <img :src="require('../'+resLunBo[7].imgSrc)">
                            <div class="leftText">
                                <h3>{{ resLunBo[7].title }}</h3>
                                <p>{{ discussArray[6] }}讨论  {{ readArray[6] }}阅读</p>
                            </div>
                        </a>
                    </div>
                    <div class="fr imgRight">
                        <img :src="require('../'+resLunBo[21].imgSrc)">
                        <img :src="require('../'+resLunBo[22].imgSrc)" style="margin-top:5px;">
                        <div class="text1">
                            <h3>#{{ resLunBo[21].title }}#</h3>
                        </div>
                        <div class="text2">
                            <h3>#{{ resLunBo[22].title }}#</h3>
                        </div>
                    </div>
                </div>
                <!-- 8 -->
                <div class="lunbo">
                    <div class="imgLeft fl">
                        <a href="#">
                            <img :src="require('../'+resLunBo[8].imgSrc)">
                            <div class="leftText">
                                <h3>{{ resLunBo[8].title }}</h3>
                                <p>{{ discussArray[7] }}讨论  {{ readArray[7] }}阅读</p>
                            </div>
                        </a>
                    </div>
                    <div class="fr imgRight">
                        <img :src="require('../'+resLunBo[23].imgSrc)">
                        <img :src="require('../'+resLunBo[24].imgSrc)" style="margin-top:5px;">
                        <div class="text1">
                            <h3>#{{ resLunBo[23].title }}#</h3>
                        </div>
                        <div class="text2">
                            <h3>#{{ resLunBo[24].title }}#</h3>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <!-- 轮播选择按钮 -->
        <div class="btnLunBo">
            <ul @click=cilckLunBo class="aa">
                <li class="item1 hong">1</li>
                <li class="item2">2</li>
                <li class="item3">3</li>
                <li class="item4">4</li>
                <li class="item5">5</li>
                <li class="item6">6</li>
                <li class="item7">7</li>
                <li class="item8">8</li>
            </ul>
        </div>
        <!-- 内容展示区 -->
        <div class="content">
            <ul>
                <li v-for="item in contentArray.slice(0, num)" :key=item.key>
                    <a href="#">
                        <!-- 判断为第一种内容展示方式 -->
                        <div class="a clearfix" v-if=item.a>
                            <div class="fl">
                                <img :src="require('../'+item.imgSrc)">
                            </div>
                            <div class="fr">
                                <p>{{ item.content }}</p>
                                <div class="xia">
                                    <img :src="require('../'+item.authorImgSrc)">
                                    <span>
                                        {{ item.author }}
                                        {{ item.time }}
                                    </span>
                                    <div class="xiaRight">
                                        <ul>
                                            <li>
                                                <i class="iconfont2">&#xe609;</i>
                                                {{ item.share }}
                                            </li>
                                            <li>|</li>
                                            <li>
                                                <i class="iconfont2">&#xe60e;</i>
                                                {{ item.comment }}
                                            </li>
                                            <li>|</li>
                                            <li>
                                                <i class="iconfont2">&#xe60c;</i>
                                                {{ item.good }}
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <!-- 判断为第二种内容展示方式 -->
                        <div class="b" v-else-if=item.b>
                            <p>{{ item.content }}</p>
                            <div class="imgDiv">
                                <img :src="require('../'+item.imgSrc1)">
                                <img :src="require('../'+item.imgSrc2)">
                                <img :src="require('../'+item.imgSrc3)">
                                <img :src="require('../'+item.imgSrc4)" style="margin-right:0px;">
                            </div>
                            <div class="xia">
                                <img :src="require('../'+item.authorImgSrc)">
                                <span>
                                        {{ item.author }}
                                        {{ item.time }}
                                </span>
                                <div class="xiaRight">
                                    <ul>
                                        <li>
                                            <i class="iconfont2">&#xe609;</i>
                                            {{ item.share }}
                                        </li>
                                        <li>|</li>
                                        <li>
                                            <i class="iconfont2">&#xe60e;</i>
                                            {{ item.comment }}
                                        </li>
                                        <li>|</li>
                                        <li>
                                            <i class="iconfont2">&#xe60c;</i>
                                            {{ item.good }}
                                        </li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                        <!-- 判断为第三种内容展示方式 -->
                        <div class="c clearfix" v-else-if=item.c>
                            <div class="fl">
                                <video controls :src="require('../'+item.imgSrc)">对不起您的浏览器不支持video标签</video>
                            </div>
                            <div class="fr">
                                <p>{{ item.content }}</p>
                                <div class="xia">
                                    <img :src="require('../'+item.authorImgSrc)">
                                    <span>
                                        {{ item.author }}
                                        {{ item.time }}
                                    </span>
                                </div>
                                <div class="xiaRight">
                                    <ul>
                                        <li>
                                            <i class="iconfont2">&#xe609;</i>
                                            {{ item.share }}
                                        </li>
                                        <li>|</li>
                                        <li>
                                            <i class="iconfont2">&#xe60e;</i>
                                            {{ item.comment }}
                                        </li>
                                        <li>|</li>
                                        <li>
                                            <i class="iconfont2">&#xe60c;</i>
                                            {{ item.good }}
                                        </li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>


<script>
import $ from 'jquery'
import remen from '@/./assets/remen.json'
import content from '@/./assets/content.json'
export default {
    data(){
        return{
            resLunBo:[],
            readArray:[],
            discussArray:[],
            contentArray:[],
            num:10
        }
    },
    methods:{
        cilckLunBo(event){
            let even = event || window.event,
                tag = even.target || even.srcElement;
            $(tag).siblings().removeClass("hong")
            $(tag).addClass("hong");
            let num = tag.innerHTML * 660 -660;
            $(".daLunBo1").css("transform","translateX(-"+num+"px)")
        },
        // 判断滚动条是否拉到底
        handleScroll(){
            if ($(document).scrollTop() >= $(document).height() - $(window).height()) {
                this.num+=5
            }
        }
    },
    mounted(){
        window.addEventListener('scroll', this.handleScroll, false)
        this.resLunBo = remen;
        // this.contentArray = content;
        for(let key in content){
            this.contentArray.push(content[key])
        }
        // 遍历阅读量
        let arrRead  =[];
        for(let key in remen){
            let num;
            if(parseInt(remen[key].read)>=1000000000){
                num = Number(remen[key].read.slice(0,3))/10 + "亿";
                arrRead.push(num)
            }else if(parseInt(remen[key].read)>=100000000){
                num = Number(remen[key].read.slice(0,2))/10 + "亿";
                arrRead.push(num)
            }else if(parseInt(remen[key].read)>=10000000){
                num = Number(remen[key].read.slice(0,5))/10 + "万";
                arrRead.push(num)
            }else if(parseInt(remen[key].read)>=1000000){
                num = Number(remen[key].read.slice(0,4))/10 + "万";
                arrRead.push(num)
            }else if(parseInt(remen[key].read)>=100000){
                num = Number(remen[key].read.slice(0,3))/10 + "万";
                arrRead.push(num)
            }else if(parseInt(remen[key].read)>=10000){
                num = Number(remen[key].read.slice(0,2))/10 + "万";
                arrRead.push(num)
            }else if(parseInt(remen[key].read)>=1000){
                num = remen[key].read.slice(0,3);
                arrRead.push(num)
            }else if(parseInt(remen[key].read)>=100){
                num = remen[key].read.slice(0,2);
                arrRead.push(num)
            }
        }
        this.readArray = arrRead;
        // 遍历讨论量
        let arrdiscuss = [];
        for(let key in remen){
            let num1;
            if(parseInt(remen[key].discuss)>=1000000000){
                num1 = Number(remen[key].discuss.slice(0,3))/10 + "亿";
                arrdiscuss.push(num1)
            }else if(parseInt(remen[key].discuss)>=100000000){
                num1 = Number(remen[key].discuss.slice(0,2))/10 + "亿";
                arrdiscuss.push(num1)
            }else if(parseInt(remen[key].discuss)>=10000000){
                num1 = Number(remen[key].discuss.slice(0,5))/10 + "万";
                arrdiscuss.push(num1)
            }else if(parseInt(remen[key].discuss)>=1000000){
                num1 = Number(remen[key].discuss.slice(0,4))/10 + "万";
                arrdiscuss.push(num1)
            }else if(parseInt(remen[key].discuss)>=100000){
                num1 = Number(remen[key].discuss.slice(0,3))/10 + "万";
                arrdiscuss.push(num1)
            }else if(parseInt(remen[key].discuss)>=10000){
                num1 = Number(remen[key].discuss.slice(0,2))/10 + "万";
                arrdiscuss.push(num1)
            }else if(parseInt(remen[key].discuss)>=1000){
                num1 = remen[key].read.slice(0,3);
                arrdiscuss.push(num1)
            }else if(parseInt(remen[key].discuss)>=100){
                num1 = remen[key].discuss.slice(0,2);
                arrdiscuss.push(num1)
            }
        }
        this.discussArray = arrdiscuss;
        // 轮播函数 和 时间
        setInterval(function(){
            let num = parseInt(document.getElementsByClassName("daLunBo1")[0].style.transform.slice(11))
            num = num -660
            // $(".daLunBo1").css("transition-duration","300ms")  
            if(num == -5280){
                // $(".daLunBo1").css("transition-duration","0ms")
                num = 0;
                $(".daLunBo1").css("transform","translateX("+num+"px)")
            }else{
                $(".daLunBo1").css("transform","translateX("+num+"px)")
            }
            hong()
        },5000)
        // 为轮播当前下标添加背景颜色
        function hong(){
            let num = parseInt(document.getElementsByClassName("daLunBo1")[0].style.transform.slice(11))
            if(num == 0){
                $(".btnLunBo .item1").addClass("hong")
                $(".btnLunBo .item2").removeClass("hong")
                $(".btnLunBo .item3").removeClass("hong")
                $(".btnLunBo .item4").removeClass("hong")
                $(".btnLunBo .item5").removeClass("hong")
                $(".btnLunBo .item6").removeClass("hong")
                $(".btnLunBo .item7").removeClass("hong")
                $(".btnLunBo .item8").removeClass("hong")
            }
            if(num == -660){
                $(".btnLunBo .item1").removeClass("hong")
                $(".btnLunBo .item2").addClass("hong")
                $(".btnLunBo .item3").removeClass("hong")
                $(".btnLunBo .item4").removeClass("hong")
                $(".btnLunBo .item5").removeClass("hong")
                $(".btnLunBo .item6").removeClass("hong")
                $(".btnLunBo .item7").removeClass("hong")
                $(".btnLunBo .item8").removeClass("hong")
            }
            if(num == -1320){
                $(".btnLunBo .item1").removeClass("hong")
                $(".btnLunBo .item2").removeClass("hong")
                $(".btnLunBo .item3").addClass("hong")
                $(".btnLunBo .item4").removeClass("hong")
                $(".btnLunBo .item5").removeClass("hong")
                $(".btnLunBo .item6").removeClass("hong")
                $(".btnLunBo .item7").removeClass("hong")
                $(".btnLunBo .item8").removeClass("hong")
            }
            if(num == -1980){
                $(".btnLunBo .item1").removeClass("hong")
                $(".btnLunBo .item2").removeClass("hong")
                $(".btnLunBo .item3").removeClass("hong")
                $(".btnLunBo .item4").addClass("hong")
                $(".btnLunBo .item5").removeClass("hong")
                $(".btnLunBo .item6").removeClass("hong")
                $(".btnLunBo .item7").removeClass("hong")
                $(".btnLunBo .item8").removeClass("hong")
            }
            if(num == -2640){
                $(".btnLunBo .item1").removeClass("hong")
                $(".btnLunBo .item2").removeClass("hong")
                $(".btnLunBo .item3").removeClass("hong")
                $(".btnLunBo .item4").removeClass("hong")
                $(".btnLunBo .item5").addClass("hong")
                $(".btnLunBo .item6").removeClass("hong")
                $(".btnLunBo .item7").removeClass("hong")
                $(".btnLunBo .item8").removeClass("hong")
            }
            if(num == -3300){
                $(".btnLunBo .item1").removeClass("hong")
                $(".btnLunBo .item2").removeClass("hong")
                $(".btnLunBo .item3").removeClass("hong")
                $(".btnLunBo .item4").removeClass("hong")
                $(".btnLunBo .item5").removeClass("hong")
                $(".btnLunBo .item6").addClass("hong")
                $(".btnLunBo .item7").removeClass("hong")
                $(".btnLunBo .item8").removeClass("hong")
            }
            if(num == -3960){
                $(".btnLunBo .item1").removeClass("hong")
                $(".btnLunBo .item2").removeClass("hong")
                $(".btnLunBo .item3").removeClass("hong")
                $(".btnLunBo .item4").removeClass("hong")
                $(".btnLunBo .item5").removeClass("hong")
                $(".btnLunBo .item6").removeClass("hong")
                $(".btnLunBo .item7").addClass("hong")
                $(".btnLunBo .item8").removeClass("hong")
            }
            if(num == -4620){
                $(".btnLunBo .item1").removeClass("hong")
                $(".btnLunBo .item2").removeClass("hong")
                $(".btnLunBo .item3").removeClass("hong")
                $(".btnLunBo .item4").removeClass("hong")
                $(".btnLunBo .item5").removeClass("hong")
                $(".btnLunBo .item6").removeClass("hong")
                $(".btnLunBo .item7").removeClass("hong")
                $(".btnLunBo .item8").addClass("hong")
            }
        }
        hong()
    }
}
</script>

<style>
@charset "utf-8";
@import '../assets/css/content.css';
#plantContent{
    width: 660px;
    /* height: 400px; */
    float: right;
    margin-right: 30px;
    /* background-color: aqua; */
    overflow: hidden;
}
/* 轮播 */
#plantContent #daLunBo{
    width: 660px;
    height: 288px;
    margin: 0px;
    padding: 0px;
}
#plantContent .daLunBo1{
    width: 5280px;
    height: 288px;
    margin: 0px;
    padding: 0px;
    transition-property: transform;
    transition-duration: 300ms;
    transition-timing-function: ease;
    transition-delay: 0ms;
    /* overflow: hidden; */
}
#plantContent .lunbo{
    width: 660px;
    height: 288px;
    margin: 0px;
    padding: 0px;
    float: left;
}
#plantContent .lunbo .imgLeft{
    position: relative;
    width: 512px;
    height: 288px;
}
#plantContent .lunbo .imgLeft a{
    display: block;
    width: 512px;
    height: 288px;
}
#plantContent .lunbo .imgLeft img{
    width: 512px;
    height: 288px;
}
#plantContent .lunbo .imgLeft .leftText{
    position: absolute;
    font-size: 12px;
    padding: 10px 8px;
    left: 0px;
    bottom: 0px;
    right:0px;
    background-color: rgba(0,0,0,.09)
}
#plantContent .lunbo .imgLeft .leftText h3{
    font-size: 18px;
    font-weight: bold;
    color: #fff;
    height: 20px;
    line-height: 20px;
    overflow: hidden;
    text-overflow:ellipsis;
    white-space: nowrap;
}
#plantContent .lunbo .imgLeft .leftText p{
    color: #fff;
    height: 20px;
    line-height: 20px;
    margin-top: 4px;
}

#plantContent .lunbo .imgRight{
    width: 140px;
    height: 288px;
    margin-left: 8px;
    position: relative;
}
#plantContent .lunbo .imgRight img{
    width: 140px;
    height: 140px;
}
#plantContent .lunbo .imgRight .text1,#plantContent .lunbo .imgRight .text2{
    position: absolute;
    max-height: 60px;
    padding: 10px 8px;
    background-color: rgba(0,0,0,.09)
}
#plantContent .lunbo .imgRight .text1{
    left: 0px;
    right: 0px;
    bottom: 145px;
    line-height: 20px;   
}
#plantContent .lunbo .imgRight .text1 h3{
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-line-clamp: 2;
    text-overflow: ellipsis;
    overflow: hidden;
    color: #fff;
    font-size: 14px;
    font-weight: bold;
}
#plantContent .lunbo .imgRight .text2{
    left: 0px;
    right: 0px;
    bottom: 0px;
    line-height: 20px;
}
#plantContent .lunbo .imgRight .text2 h3{
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-line-clamp: 2;
    text-overflow: ellipsis;
    overflow: hidden;
    color: #fff;
    font-size: 14px;
    font-weight: bold;
}

/* 轮播选择按钮 */
#plantContent .btnLunBo{
    width: 128px;
    height: 6px;
    text-align: center;
    margin: 10px auto;
}
#plantContent .btnLunBo ul{
    margin: 0 auto;
}
#plantContent .btnLunBo li{
   list-style: none;
   float: left; 
   margin: 0 5px;
   background-color: #ccc;
   border-radius: 50%;
   width: 6px;
   height: 6px;
   text-indent: -999999px;
   cursor: pointer;
}
#plantContent .btnLunBo li.hong{
    background-color: #eb7350;
}


/* 内容展示区 */
#plantContent .content{
    width: 660px;
    height: 800px;
    /* background-color: red; */
}
#plantContent .content li{
    list-style: none;
    padding: 0;
    margin: 0;
    margin-bottom: 10px;
}
#plantContent .content a{
    width: 660px;
    display: block;
}
#plantContent .content .a{
    box-sizing: border-box;
    width: 660px;
    height: 113px;
    border-bottom: 1px solid #aaaaaa;
}
#plantContent .content .a .fl{
    width: 158px;
    height: 102px;
}
#plantContent .content .a .fl img{
    width: 158px;
    height: 102px;
}
#plantContent .content .a .fr{
    width: 489px;
    height: 102px;
    padding: 10px 0px;
}
#plantContent .content .a .fr p{
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-line-clamp: 2;
    text-overflow: ellipsis;
    overflow: hidden;
    line-height: 24px;
    font-size: 14px;
    max-height: 48px;
    margin-bottom: 14px;
}
#plantContent .content .a .fr .xia{
    width: 489px;
    margin: 0;
    padding: 0;
    height: 20px;
    position: relative;
}
#plantContent .content .a .fr .xia img{
    width: 20px;
    height: 20px;
    border-radius: 50%;
}
#plantContent .content .a .fr .xia span{
    position: absolute;
    margin-left: 5px;
    bottom: 0;
    line-height: 20px;
    color:#9c9c9c;
}
#plantContent .content .a .fr .xia .xiaRight{
    position: absolute;
    bottom: 0px;
    right: 0px;
    height: 20px;
}
#plantContent .content .a .fr .xia .xiaRight li{
    color: #9c9c9c;
    float: left;
    height: 20px;
    line-height: 20px;
    list-style: none;
    margin-left: 5px;
}
#plantContent .content .a .fr .xia .xiaRight li i{
    color: #9c9c9c;
    font-size: 16px;
}
#plantContent .content .a .fr .xia .xiaRight li i:hover{
    color: #eb7350;
}

#plantContent .content .b{
    box-sizing: border-box;
    width: 660px;
    height: 177px;
    padding-bottom: 10px;
    border-bottom: 1px solid #aaaaaa;
}
#plantContent .content .b p{
    word-break: keep-all;
    height: 24px;
    line-height: 24px;
    font-size: 14px;
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-line-clamp: 1;
    text-overflow: ellipsis;
    overflow: hidden;
}
#plantContent .content .b .imgDiv{
    width: 660px;
    height: 102px;
    margin-top: 10px;
}
#plantContent .content .b .imgDiv img{
    width: 158px;
    height: 102px;
    margin-right: 9.3px;
}
#plantContent .content .b .xia{
    width: 660px;
    height: 20px;
    margin-top: 10px;
    margin-bottom: 10px;
    position: relative;
}
#plantContent .content .b .xia img{
    width: 20px;
    height: 20px;
    border-radius: 50%;
}
#plantContent .content .b .xia span{
    position: absolute;
    margin-left: 5px;
    bottom: 0;
    line-height: 20px;
    color:#9c9c9c;
}
#plantContent .content .b .xia .xiaRight{
    position: absolute;
    bottom: 0px;
    right: 0px;
    height: 20px;
}
#plantContent .content .b .xia .xiaRight li{
    color: #9c9c9c;
    float: left;
    height: 20px;
    line-height: 20px;
    list-style: none;
    margin-left: 5px;
}
#plantContent .content .b .xia .xiaRight li i{
    color: #9c9c9c;
    font-size: 16px;
}
#plantContent .content .b .xia .xiaRight li i:hover{
    color: #eb7350;
}

#plantContent .content .c{
    box-sizing: border-box;
    width: 660px;
    height: 195px;
    padding-bottom: 10px;
    border-bottom: 1px solid #aaaaaa;
}
#plantContent .content .c .fl video{
    width: 326px;
    height: 184px;
}
#plantContent .content .c .fr{
    width: 308px;
    height: 184px;
    margin-left: 26px;
    position: relative;
}
#plantContent .content .c .fr p{
    word-break: keep-all;
    line-height: 24px;
    font-size: 14px;
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-line-clamp: 4;
    text-overflow: ellipsis;
    overflow: hidden;
}
#plantContent .content .c .fr .xia{
    margin-top: 10px;
    position: relative;
}
#plantContent .content .c .fr .xia img{
    width: 20px;
    height: 20px;
    border-radius: 50%;
}
#plantContent .content .c .fr .xia span{
    line-height: 20px;
    color:#9c9c9c;
    position: absolute;
    bottom: 0px;
    margin-left: 5px;
}
#plantContent .content .c .fr .xiaRight{
    position: absolute;
    bottom: 0px;
    right: 0px;
    height: 20px;
}
#plantContent .content .c .fr .xiaRight li{
    color: #9c9c9c;
    float: left;
    height: 20px;
    line-height: 20px;
    list-style: none;
    margin-left: 5px;
}
#plantContent .content .c .fr .xiaRight li i{
    color: #9c9c9c;
    font-size: 16px;
}
#plantContent .content .c .fr .xiaRight li i:hover{
    color: #eb7350;
}

</style>