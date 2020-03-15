<template>
    <div id="foot">
        <div class="foot1">
            <dl class="list list1">
                <dt>微博精彩</dt>
                <dd>
                    <span><a href="#">热门微博</a></span>
                    <span><a href="#">热门话题</a></span>
                </dd>
                <dd>
                    <span><a href="#">名人堂</a></span>
                    <span><a href="#">微博会员</a></span>
                </dd>
                <dd>
                    <span><a href="#">微相册</a></span>
                    <span><a href="#">微游戏</a></span>
                </dd>
                <dd>
                    <span><a href="#">微指数</a></span>
                </dd>
            </dl>
            <dl class="list list2">
                <dt>手机玩微博</dt>
                <dd>
                    <span>
                        <img :src="require('../assets/image/footCode.png')">
                    </span>
                </dd>
                <dd>
                    <span style="margin:0px">
                        扫码下载，更多版本<br>
                        戳这里
                    </span>
                </dd>
            </dl>
            <dl class="list list3">
                <dt>认证&合作</dt>
                <dd>
                    <span><a href="#">申请认证</a></span>
                    <span><a href="#">链接网站</a></span>
                </dd>
                <dd>
                    <span><a href="#">企业微博</a></span>
                    <span><a href="#">广告服务</a></span>
                </dd>
                <dd>
                    <span><a href="#">微博标识</a></span>
                    <span><a href="#">广告代理商</a></span>
                </dd>
                <dd>
                    <span><a href="#">开放平台</a></span>
                </dd>
            </dl>
            <dl class="list list4">
                <dt>微博帮助</dt>
                <dd>
                    <span><a href="#">常见问题</a></span>
                </dd>
                <dd>
                    <span><a href="#">自助服务</a></span>
                </dd>
                <dd>
                    <span>企业&商业热线</span>
                </dd>
                <dd>
                    <span>4000-980-980</span>
                </dd>
            </dl>
        </div>
        <div class="foot2">
            <p>
                <span>微博客服</span>
                <span>客服热线4000-960-960</span>
                <span>意见反馈</span>
                <span>舞弊举报</span>
                <span>开放平台</span>
                <span>微博招聘</span>
                <span>新浪网导航</span>
                <span>投诉处理大厅</span>
                <span>DMCA投诉/Report</span>
            </p>
            <p>
                <span><a href="#">京ICP证100780号</a></span>
                <span>互联网药品服务许可证</span>
                <span>互联网医疗保健许可证</span>
                <span>京网文[2017]10291-1172号</span>
                <span><a href="#">京ICP备12002058号</a></span>
                <span>增值电信业务经营许可证B2-20140447</span>
            </p>
            <p>
                <span>互联网新闻信息服务许可编号:11220190001</span>
                <span>Copyright © 2009-2020 WEIBO <a href="#">北京微梦创科网络技术有限公司</a></span>
                <span><a href="#">京公网安备11000002000019号</a></span>
            </p>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style>
#foot{
    width: 100%;
    border-top: 1px solid #9c9c9c;
    margin-top: 10px;
}
#foot a:hover{
    color: #eb7350;
}
#foot .foot1{
    width: 920px;
    margin: 0 auto;
    padding: 20px 0 10px 80px;
    height: 123px;
    /* background-color: aqua; */
}
#foot .foot1 a{
    color: #808080;
}
#foot .foot1 a:hover{
    color: #eb7350;
}
#foot .foot1 .list{
    float: left;
    margin: 0 70px 0 0;
}
#foot .foot1 .list dt{
    font-size: 16px;
    padding: 0 0 15px;
    white-space: nowrap;
    width: 138px;
    overflow: hidden;
}
#foot .foot1 .list1 span{
    display: inline-block;
    width: 48px;
    margin: 0 20px 5px 0;
    color: #808080;
}
#foot .foot1 .list2 dd{
    float: left;
}
#foot .foot1 .list2 span{
    display: inline-block;
    margin: 0 10px 5px 0;
    color: #808080;
}
#foot .foot1 .list2 span img{
    width: 79px;
    height: 79px;
}
#foot .foot1 .list3 span{
    display: inline-block;
    width: 60px;
    margin: 0 20px 5px 0;
    color: #808080;
}
#foot .foot1 .list4 span{
    display: inline-block;
    width: 122px;
    margin: 0 20px 5px 0;
    color: #808080;
}

#foot .foot2{
    width: 100%;
    text-align: center;
    padding: 20px 0 45px;
    background-color: #f2f2f5;
    height: 72px;

}
#foot .foot2 p{
    margin-bottom: 10px;
}
#foot .foot2 p span{
    margin-right: 15px;
}
</style>