<template>
    <div id="rightNav">
        <!-- 登录 -->
        <div class="sign">
            <div class="sign1">
                <ul>
                    <li class="hong" @click=clickTrue>账号登录</li>
                    <li @click=clickFalse>手机登录</li>
                </ul>
                <div class="form">
                    <form action="#" method="get">
                        <div class="yonghuming" v-if=tureORflase>
                            <span class="iconfont1">&#xe610;</span>
                            <input type="text" id="haoma" required autocomplete="off" placeholder="邮箱/会员账号/手机号">
                        </div>
                        <div class="shouji" v-else>
                            <span class="iconfont1">&#xe618;</span>
                            <input type="text" id="haoma" required autocomplete="off" placeholder="手机号码，仅支持大陆手机">
                        </div>

                        <div class="mima" v-if=tureORflase>
                            <span class="iconfont1">&#xe60d;</span>
                            <input type="password" id="mima" required placeholder="请输入密码">
                        </div>
                        <div class="erweima" v-else>
                            <button>获取短信验证码</button>
                            <input type="text" id="mima" autocomplete="off" placeholder="短信验证码">
                        </div>

                        <div class="danxuan clearfix">
                            <div class="fl">
                                <input type="checkbox" id="jizhuwo" value="记住我">&nbsp;&nbsp;&nbsp;<label for="jizhuwo" style="color:#9c9c9c;">记住我</label>
                            </div>
                            <div class="fr">
                                <a href="#">忘记密码</a>
                            </div>
                        </div>
                        <div class="btn">
                            <input type="submit" value="登录">
                        </div>
                        <div class="dibu">
                            还没有微博？<a href="#">立即注册!</a>
                        </div>
                    </form>
                </div>
                <div class="qita">
                    其他登录：<a href="#" class="iconfont1">&#xe608;</a>
                    <a href="#" class="iconfont1">&#xe60a;</a>
                    <a href="#" class="iconfont1">&#xe615;</a>
                    <a href="#" class="iconfont1">&#xe602;</a>
                </div>
            </div>
        </div>
        <!-- 热门 -->
        <div class="remen">
            <div class="remen1">
                <h3>微博热门话题</h3>
                <ul>
                    <li>
                        <a href="#">
                            <img :src="require('../'+res[9].imgSrc)">
                            <div>
                                <h4>#{{ res[9].title }}#</h4>
                                <span>{{ readArray[8] }}阅读&nbsp;{{ discussArray[8] }}讨论</span>
                            </div>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img :src="require('../'+res[10].imgSrc)">
                            <div>
                                <h4>#{{ res[10].title }}#</h4>
                                <span>{{ readArray[9] }}阅读&nbsp;{{ discussArray[9] }}讨论</span>
                            </div>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img :src="require('../'+res[11].imgSrc)">
                            <div>
                                <h4>#{{ res[11].title }}#</h4>
                                <span>{{ readArray[10]}}阅读&nbsp;{{ discussArray[10] }}讨论</span>
                            </div>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img :src="require('../'+res[12].imgSrc)">
                            <div>
                                <h4>#{{ res[12].title }}#</h4>
                                <span>{{ readArray[11] }}阅读&nbsp;{{ discussArray[11] }}讨论</span>
                            </div>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img :src="require('../'+res[13].imgSrc)">
                            <div>
                                <h4>#{{ res[13].title }}#</h4>
                                <span>{{ readArray[12] }}阅读&nbsp;{{ discussArray[12] }}讨论</span>
                            </div>
                        </a>
                    </li>
                </ul>
            </div>
            <div class="more">
                <a href="#">查看更多>></a>
            </div>
        </div>
        <!-- 热点 -->
        <div class="redian">
            <div class="redian1">
                <h3>微博实时热点</h3>
                <ul>
                    <li>
                        <a href="#">
                            <img :src="require('../'+resRedian[1].imgSrc)">
                            <div>
                                <h4>#{{ resRedian[1].title }}#</h4>
                                <span>{{ resRedian[1].content }}</span>
                            </div>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img :src="require('../'+resRedian[2].imgSrc)">
                            <div>
                                <h4>#{{ resRedian[2].title }}#</h4>
                                <span>{{ resRedian[2].content }}</span>
                            </div>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img :src="require('../'+resRedian[3].imgSrc)">
                            <div>
                                <h4>#{{ resRedian[3].title }}#</h4>
                                <span>{{ resRedian[3].content }}</span>
                            </div>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img :src="require('../'+resRedian[4].imgSrc)">
                            <div>
                                <h4>#{{ resRedian[4].title }}#</h4>
                                <span>{{ resRedian[4].content }}</span>
                            </div>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img :src="require('../'+resRedian[5].imgSrc)">
                            <div>
                                <h4>#{{ resRedian[5].title }}#</h4>
                                <span>{{ resRedian[5].content }}</span>
                            </div>
                        </a>
                    </li>
                </ul>
            </div>
            <div class="more">
                <a href="#">查看更多>></a>
            </div>
        </div>
        <!-- 微博找人 -->
        <div class="zhaoren">
            <h3>微博找人</h3>
            <!-- 名人 -->
            <div class="mingren">
                <h4>名人</h4>
                <ul>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe8b3;</i>
                            <span>明星</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe629;</i>
                            <span>商界</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe619;</i>
                            <span>媒体精英</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe625;</i>
                            <span>作家</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe60c;</i>
                            <span>政府官员</span>
                        </a>
                    </li>
                </ul>
            </div>
            <!-- 专家 -->
            <div class="zhuanjia">
                <h4>专家</h4>
                <ul>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe6ee;</i>
                            <span>医疗</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe617;</i>
                            <span>育儿</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe612;</i>
                            <span>IT互联网</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe621;</i>
                            <span>电台</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe658;</i>
                            <span>财经</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe61d;</i>
                            <span>教育</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe61a;</i>
                            <span>法律</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe628;</i>
                            <span>美妆</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe607;</i>
                            <span>艺术</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe604;</i>
                            <span>设计</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe614;</i>
                            <span>房产家装</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe71d;</i>
                            <span>汽车</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe622;</i>
                            <span>交通</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe6d0;</i>
                            <span>职业招聘</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe611;</i>
                            <span>婚庆</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe62e;</i>
                            <span>宗教</span>
                        </a>
                    </li>
                </ul>
            </div>
            <!-- 兴趣 -->
            <div class="xingqu">
                <h4>专家</h4>
                <ul>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe619;</i>
                            <span>时尚</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe627;</i>
                            <span>美女</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe65b;</i>
                            <span>电影</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe61b;</i>
                            <span>电视剧</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe63b;</i>
                            <span>音乐</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe620;</i>
                            <span>动漫</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe6b3;</i>
                            <span>游戏</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe62c;</i>
                            <span>星座</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe616;</i>
                            <span>搞笑</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe62a;</i>
                            <span>情感两性</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe60f;</i>
                            <span>运动健身</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe62b;</i>
                            <span>体育</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe603;</i>
                            <span>萌宠</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe61c;</i>
                            <span>美食</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe647;</i>
                            <span>旅游</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe633;</i>
                            <span>摄影</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe659;</i>
                            <span>历史</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe624;</i>
                            <span>军事</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe626;</i>
                            <span>科学</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe618;</i>
                            <span>数码</span>
                        </a>
                    </li>
                </ul>
            </div>
            <!-- 机构 -->
            <div class="jigou">
                <h4>机构</h4>
                <ul>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe62d;</i>
                            <span>政务</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="iconfont1">&#xe636;</i>
                            <span>媒体</span>
                        </a>
                    </li>
                </ul>
            </div>
        </div>
        <!-- 投诉 -->
        <div class="touSu">
            <a href="#">DMCA投诉/Reporta ></a>
        </div>

        <!-- 隐藏的登录 -->
        <div class="sign signa">
            <div class="sign1">
                <ul>
                    <li class="hong" @click=clickTrue>账号登录</li>
                    <li @click=clickFalse>手机登录</li>
                </ul>
                <div class="form">
                    <form action="#" method="get">
                        <div class="yonghuming" v-if=tureORflase>
                            <span class="iconfont1">&#xe610;</span>
                            <input type="text" id="haoma2" required autocomplete="off" placeholder="邮箱/会员账号/手机号">
                        </div>
                        <div class="shouji" v-else>
                            <span class="iconfont1">&#xe618;</span>
                            <input type="text" id="haoma2" required autocomplete="off" placeholder="手机号码，仅支持大陆手机">
                        </div>

                        <div class="mima" v-if=tureORflase>
                            <span class="iconfont1">&#xe60d;</span>
                            <input type="password" id="mima2" required placeholder="请输入密码">
                        </div>
                        <div class="erweima" v-else>
                            <button>获取短信验证码</button>
                            <input type="text" id="mima2" autocomplete="off" placeholder="短信验证码">
                        </div>

                        <div class="danxuan clearfix">
                            <div class="fl">
                                <input type="checkbox" id="jizhuwo2" value="记住我">&nbsp;&nbsp;&nbsp;<label for="jizhuwo" style="color:#9c9c9c;">记住我</label>
                            </div>
                            <div class="fr">
                                <a href="#">忘记密码</a>
                            </div>
                        </div>
                        <div class="btn">
                            <input type="submit" value="登录">
                        </div>
                        <div class="dibu">
                            还没有微博？<a href="#">立即注册!</a>
                        </div>
                    </form>
                </div>
                <div class="qita">
                    其他登录：<a href="#" class="iconfont1">&#xe608;</a>
                    <a href="#" class="iconfont1">&#xe60a;</a>
                    <a href="#" class="iconfont1">&#xe615;</a>
                    <a href="#" class="iconfont1">&#xe602;</a>
                </div>
            </div>
        </div>

        <!-- 返回顶部 -->
        <div class="fanhui" @click=clickFanHui>
            返回 顶部
        </div>
    </div>
</template>


<script>
import $ from 'jquery'
import remen from '@/./assets/remen.json'
import redian from '@/./assets/redian.json'
export default {
    data(){
        return{
            res:[],
            resRedian:[],
            tureORflase:true,
            readArray:[],
            discussArray:[],
            hideDengLu:false
        }
    },
    methods:{
        clickTrue:function(event){
            let even = event || window.event,
                tag = even.target || even.srcElement;
            this.tureORflase = true;
            $(tag).addClass("hong")
            $(tag).siblings().removeClass("hong")
        },
        clickFalse:function(event){
            let even = event || window.event,
                tag = even.target || even.srcElement;
            this.tureORflase = false;
            $(tag).addClass("hong")
            $(tag).siblings().removeClass("hong")
        },
        clickFanHui:function(){
            $(document).scrollTop(0)
        },
        // 判断滚动条是否拉到底
        handleScroll(){
            if ($(document).scrollTop() >= $(document).height() - $(window).height()) {
                $(".fanhui").css("bottom","310px")
            }else{
                $(".fanhui").css("bottom","40px")
            }
        }
    },
    mounted(){
        window.addEventListener('scroll', this.handleScroll, false)
        this.res = remen;
        this.resRedian = redian;
        $(document).scroll(function(){
            let res = $(this).scrollTop();
            if(res >= 5){
                $(".fanhui").css("visibility","visible")
            }else{
                $(".fanhui").css("visibility","hidden")
            }
            if(res >= 2220){
                $(".signa").css("visibility","visible")
            }else{
                $(".signa").css("visibility","hidden")
            }
        })        
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
                num = remen[key].read.slice(0,4);
                arrRead.push(num)
            }else if(parseInt(remen[key].read)>=100){
                num = remen[key].read.slice(0,3);
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
                num1 = remen[key].discuss.slice(0,4);
                arrdiscuss.push(num1)
            }else if(parseInt(remen[key].discuss)>=100){
                num1 = remen[key].discuss.slice(0,3);
                arrdiscuss.push(num1)
            }
        }
        this.discussArray = arrdiscuss;
    }
}
</script>

<style>
@charset "utf-8";
@import '../assets/css/rightNav.css';
#rightNav{
    width: 340px;
    /* height: 300px; */
    float: right;
}
/* 登录 */
#rightNav .signa{
    position: fixed;
    top: 60px;
    visibility:hidden;
}
#rightNav .sign{
    box-sizing: border-box;
    width: 340px;
    height: 326px;
    background-color: #f2f2f5;
    padding: 20px;
}
#rightNav .sign .sign1{
    box-sizing: border-box;
    width: 300px;
    height: 286px;
    /* margin: 0 auto; */
    border: 1px solid #efefef;
    background-color: #fff;
    padding: 0 10px;
    /* margin-bottom: 16px; */
}
#rightNav .sign .sign1 ul li{
    box-sizing: border-box;
    float: left;
    list-style: none;
    text-align: center;
    font-size: 14px;
    color: #9c9c9c;
    width: 135px;
    height: 44px;
    line-height: 44px;
    border-bottom: 1px solid #efefef;
}
#rightNav .sign .sign1 ul li:hover{
    cursor: pointer;
}
#rightNav .sign .sign1 ul li.hong{
    color: #333;
    border-bottom: 2px solid #ff8140;
}

#rightNav .sign .sign1 .form{
    width: 270px;
    height: 191px;
    box-sizing: border-box;
    border-bottom: 1px solid #efefef;
    margin-top: 60px;
}
#rightNav .sign .sign1 .form .yonghuming{
    border-radius: 2px;
    padding-top:2px; 
    width: 270px;
    height: 34px;
    box-sizing: border-box;
    border: 1px solid #efefef;
}
#rightNav .sign .sign1 .form .yonghuming span{
    text-align: center;
    display: inline-block;
    font-size: 20px;
    width: 12%;
    height: 28px;
    line-height: 28px;
}
#rightNav .sign .sign1 .form .yonghuming input{
    width: 85%;
    height: 24px;
    line-height: normal;
    margin-bottom: 8px;
    vertical-align: middle;
    border: none;
    box-shadow: none;
    outline: none;
}
#rightNav .sign .sign1 .form .shouji{
    border-radius: 2px;
    padding-top:2px; 
    width: 270px;
    height: 34px;
    box-sizing: border-box;
    border: 1px solid #efefef;
}
#rightNav .sign .sign1 .form .shouji span{
    text-align: center;
    display: inline-block;
    font-size: 20px;
    width: 12%;
    height: 28px;
    line-height: 28px;
}
#rightNav .sign .sign1 .form .shouji input{
    width: 85%;
    height: 24px;
    line-height: normal;
    margin-bottom: 8px;
    vertical-align: middle;
    border: none;
    box-shadow: none;
    outline: none;
}

#rightNav .sign .sign1 .form .mima{
    border-radius: 2px;
    padding-top:2px; 
    width: 270px;
    height: 34px;
    box-sizing: border-box;
    border: 1px solid #efefef;
    margin-top: 12px;
}
#rightNav .sign .sign1 .form .mima span{
    text-align: center;
    display: inline-block;
    font-size: 20px;
    width: 12%;
    height: 28px;
    line-height: 28px;
}
#rightNav .sign .sign1 .form .mima input{
    width: 85%;
    height: 24px;
    line-height: normal;
    margin-bottom: 8px;
    vertical-align: middle;
    border: none;
    box-shadow: none;
    outline: none;
}
#rightNav .sign .sign1 .form .erweima{
    padding-top:2px; 
    width: 270px;
    height: 34px;
    box-sizing: border-box;
    margin-top: 12px;
}
#rightNav .sign .sign1 .form .erweima button{
    box-sizing: border-box;
    width: 143px;
    height: 34px;
    background-color: #f2f2f5;
    border: 1px solid #efefef;
    border-radius: 2px;
}
#rightNav .sign .sign1 .form .erweima button:hover{
    cursor: pointer;
    background-color: #9c9c9c;
}
#rightNav .sign .sign1 .form .erweima input{
    border: 1px solid #efefef;
    border-radius: 2px;
    margin-left: 10px;
    box-sizing: border-box;
    width: 116px;
    height: 34px;
    outline-color: #ff8140
}

#rightNav .sign .sign1 .form .danxuan{
    padding-top:2px; 
    width: 270px;
    height: 15px;
    line-height: 15px;
    box-sizing: border-box;
    margin-top: 12px;
    color: #9c9c9c;
}
#rightNav .sign .sign1 .form .danxuan input{
    vertical-align: middle;
}
#rightNav .sign .sign1 .form .danxuan a{
    color:#9c9c9c;
}
#rightNav .sign .sign1 .form .danxuan a:hover{
    color:#ff8140;
}

#rightNav .sign .sign1 .form .btn{
    width: 270px;
    height: 34px;
    box-sizing: border-box;
    margin-top: 12px;
    background-color: #ff8140;
    border-radius: 2px;
}
#rightNav .sign .sign1 .form .btn input{
    width: 270px;
    height: 34px;
    background-color: #ff8140;
    border-radius: 2px;
    line-height: 34px;
    text-align: center;
    border: 1px solid #f77c3d;
    font-size: 16px;
    font-weight: bold;
    color: #fff;
    box-shadow: 0px 1px 2px rgba(0,0,0,0.25);
}
#rightNav .sign .sign1 .form .btn input:hover{
    cursor: pointer;
    background-color: #eb7350;
}
#rightNav .sign .sign1 .form .dibu{
    width: 270px;
    height: 26px;
    box-sizing: border-box;
    margin-top: 12px;
    color: #9c9c9c;
}
#rightNav .sign .sign1 .form .dibu a{
    color: #eb7350;
}

#rightNav .sign .sign1 .qita{
    width: 270px;
    height: 16px;
    line-height: 16px;
    margin-top: 10px;
    color: #9c9c9c;
}
#rightNav .sign .sign1 .qita a{
    color: #ff8140;
    margin-left: 10px;
}


/* 热门 */
#rightNav .remen{
    box-sizing: border-box;
    width: 340px;
    height: 444px;
    border-top:1px solid #fb3c31;
    margin-top: 20px;
    background-color: #f2f2f5;
}
#rightNav .remen .remen1{
    box-sizing: border-box;
    width: 340px;
    height: 410px;
    padding: 20px;
}
#rightNav .remen .remen1 h3{
    font-size: 18px;
    font-weight: 700;
    margin-bottom: 16px;
}
#rightNav .remen .remen1 li{
    width: 300px;
    list-style: none;
    height: 50px;
    margin-top: 20px;
}
#rightNav .remen .remen1 li a{
    display: block;
    width: 300px;
    height: 50px;
}
#rightNav .remen .remen1 li a img{
    float: left;
    width: 50px;
    height: 50px;
}
#rightNav .remen .remen1 li a div{
    /* padding-top:  */
    /* margin-top: 6px; */
    margin-left: 12px;
    float: right;
    width: 238px;
    height: 44px;
}
#rightNav .remen .remen1 li a div h4{
    width: 238px;
    overflow: hidden;
    font-weight: normal;
    font-size: 14px;
    height: 22px;
    line-height: 22px;
    text-overflow:ellipsis;
    white-space: nowrap;
}
#rightNav .remen .remen1 li a div h4:hover{
    color: #ff8140;
    cursor: pointer;
}
#rightNav .remen .remen1 li a div span{
    display: inline-block;
    margin-top: 5px;
    color: #9c9c9c;
    height: 22px;
    line-height: 22px;
    width: 238px;
    overflow: hidden;
}
#rightNav .remen .more{
    box-sizing: border-box;
    width: 340px;
    height: 34px;
    line-height: 34px;
    border-top: 1px solid #9c9c9c;
    text-align: center;
}
#rightNav .remen .more a{
    display: inline-block;
    width: 340px;
    height: 34px;
    line-height: 34px;
}


/* 热点 */
#rightNav .redian{
    box-sizing: border-box;
    width: 340px;
    height: 444px;
    border-top:1px solid #fb3c31;
    margin-top: 20px;
    background-color: #f2f2f5;
}
#rightNav .redian .redian1{
    box-sizing: border-box;
    width: 340px;
    height: 410px;
    padding: 20px;
}
#rightNav .redian .redian1 h3{
    font-size: 18px;
    font-weight: 700;
    margin-bottom: 16px;
}
#rightNav .redian .redian1 li{
    width: 300px;
    list-style: none;
    height: 50px;
    margin-top: 20px;
}
#rightNav .redian .redian1 li a{
    display: block;
    width: 300px;
    height: 50px;
}
#rightNav .redian .redian1 li a img{
    float: left;
    width: 50px;
    height: 50px;
}
#rightNav .redian .redian1 li a div{
    /* padding-top:  */
    /* margin-top: 6px; */
    margin-left: 12px;
    float: right;
    width: 238px;
    height: 44px;
}
#rightNav .redian .redian1 li a div h4{
    width: 238px;
    overflow: hidden;
    text-overflow:ellipsis;
    white-space: nowrap;
    font-weight: normal;
    font-size: 14px;
    height: 22px;
    line-height: 22px;
}
#rightNav .redian .redian1 li a div h4:hover{
    color: #ff8140;
    cursor: pointer;
}
#rightNav .redian .redian1 li a div span{
    display: inline-block;
    margin-top: 5px;
    color: #9c9c9c;
    height: 22px;
    line-height: 22px;
    width: 238px;
    overflow: hidden;
    text-overflow:ellipsis;
    white-space: nowrap;
}
#rightNav .redian .more{
    box-sizing: border-box;
    width: 340px;
    height: 34px;
    line-height: 34px;
    border-top: 1px solid #9c9c9c;
    text-align: center;
}
#rightNav .redian .more a{
    display: inline-block;
    width: 340px;
    height: 34px;
    line-height: 34px;
}


/* 微博找人 */
#rightNav .zhaoren{
    box-sizing: border-box;
    width: 340px;
    height: 827px;
    border-top:1px solid #fb3c31;
    margin-top: 20px;
    background-color: #f2f2f5;
    padding: 20px;
}
#rightNav .zhaoren h3{
    font-size: 18px;
    font-weight: 700;
    margin-bottom: 16px;
}
#rightNav .zhaoren .mingren{
    box-sizing: border-box;
    width: 300px;
    height: 107px;
    border-bottom: 1px solid #9c9c9c;
    color: #9c9c9c;
}
#rightNav .zhaoren .mingren h4{
    font-size: 16px;
    font-weight: normal;
    color: #9c9c9c;
    margin-bottom: 16px;
}
#rightNav .zhaoren .mingren li{
    height: 15px;
    line-height: 15px;
    list-style: none;
    width: 33.3%;
    margin-bottom: 20px;
    float: left;
}
#rightNav .zhaoren .mingren li i{
    color: #9c9c9c;
}
#rightNav .zhaoren .mingren li i:hover{
    cursor: pointer;
}
#rightNav .zhaoren .mingren li span{
    margin-left: 5px;
    display: inline-block;
    vertical-align: middle;
    line-height: 14px;
    color: #9c9c9c;
}
#rightNav .zhaoren .mingren li span:hover{
    color: #ff8140;
    cursor: pointer;
}

#rightNav .zhaoren .zhuanjia{
    box-sizing: border-box;
    margin-top: 20px;
    width: 300px;
    height: 247px;
    border-bottom: 1px solid #9c9c9c;
}
#rightNav .zhaoren .zhuanjia h4{
    font-size: 16px;
    font-weight: normal;
    color: #9c9c9c;
    margin-bottom: 16px;
}
#rightNav .zhaoren .zhuanjia li{
    height: 15px;
    line-height: 15px;
    list-style: none;
    width: 33.3%;
    margin-bottom: 20px;
    float: left;
}
#rightNav .zhaoren .zhuanjia li i{
    color: #9c9c9c;
}
#rightNav .zhaoren .zhuanjia li i:hover{
    cursor: pointer;
}
#rightNav .zhaoren .zhuanjia li span{
    margin-left: 5px;
    display: inline-block;
    vertical-align: middle;
    line-height: 14px;
    color: #9c9c9c;
}
#rightNav .zhaoren .zhuanjia li span:hover{
    color: #ff8140;
    cursor: pointer;
}

#rightNav .zhaoren .xingqu{
    box-sizing: border-box;
    margin-top: 20px;
    width: 300px;
    height: 282px;
    border-bottom: 1px solid #9c9c9c;
}
#rightNav .zhaoren .xingqu h4{
    font-size: 16px;
    font-weight: normal;
    color: #9c9c9c;
    margin-bottom: 16px;
}
#rightNav .zhaoren .xingqu li{
    height: 15px;
    line-height: 15px;
    list-style: none;
    width: 33.3%;
    margin-bottom: 20px;
    float: left;
}
#rightNav .zhaoren .xingqu li i{
    color: #9c9c9c;
}
#rightNav .zhaoren .xingqu li i:hover{
    cursor: pointer;
}
#rightNav .zhaoren .xingqu li span{
    margin-left: 5px;
    display: inline-block;
    vertical-align: middle;
    line-height: 14px;
    color: #9c9c9c;
}
#rightNav .zhaoren .xingqu li span:hover{
    color: #ff8140;
    cursor: pointer;
}

#rightNav .zhaoren .jigou{
    box-sizing: border-box;
    margin-top: 20px;
    width: 300px;
    height: 71px;
}
#rightNav .zhaoren .jigou h4{
    font-size: 16px;
    font-weight: normal;
    color: #9c9c9c;
    margin-bottom: 16px;
}
#rightNav .zhaoren .jigou li{
    height: 15px;
    line-height: 15px;
    list-style: none;
    width: 33.3%;
    margin-bottom: 20px;
    float: left;
}
#rightNav .zhaoren .jigou li i{
    color: #9c9c9c;
}
#rightNav .zhaoren .jigou li i:hover{
    cursor: pointer;
}
#rightNav .zhaoren .jigou li span{
    margin-left: 5px;
    display: inline-block;
    vertical-align: middle;
    line-height: 14px;
    color: #9c9c9c;
}
#rightNav .zhaoren .jigou li span:hover{
    color: #ff8140;
    cursor: pointer;
}


/* 投诉 */
#rightNav .touSu{
    box-sizing: border-box;
    padding:20px;
    width: 340px;
    height: 57px;
    border-top:1px solid #fb3c31;
    margin-top: 20px;
    background-color: #f2f2f5;
}


/* 返回顶部 */
#rightNav .fanhui{
    width: 50px;
    height: 50px;
    line-height: 25px;
    text-align: center;
    position: fixed;
    bottom: 40px;
    background-color: #9c9c9c; 
    margin-left: 345px;
    word-break: keep-all;
    cursor: pointer;
    font-size: 12px;
    color: #fff;
    font-weight: bold;
    visibility:hidden;
}
#rightNav .fanhui:hover{
    background-color: #696e78;
}

</style>