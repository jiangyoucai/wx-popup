# wx-popup
微信小程序弹出层组件（a popup component for wechat miniprogram）

# 使用

1.复制文件

    复制plugin/components/popup 文件夹到项目中

2.引入组件

    pages/index/index.json文件里，增加
    
    {
    "usingComponents": {
    "popup": "your path/popup"
    }

3.使用组件

    pages/index/index.wxml文件里，增加
    
    <popup option="{{option}}">
      <view slot="action">
        <text>购物车</text>
      </view>
      <view slot="data" class="container x92 x-column">
        <text>1bind:setSKU="setSKU" bind:setBooking="setBooking"1bind:setSKU="setSKU" bind:setBooking="setBooking"</text>
        <text>x</text>
        <text>y</text>
        <text>z</text>
        <text>2</text>
        <text>x</text>
        <text>y</text>
        <text>z</text>
        <text>3</text>
        <text>x</text>
        <text>y</text>
        <text>z</text>
        <text>4</text>
        <text>x</text>
        <text>y</text>
        <text>z</text>
        <text>5</text>
        <text>x</text>
        <text>y</text>
        <text>z</text>
        <text>6</text>
        <text>x</text>
        <text>y</text>
        <text>z</text>
      </view>
    </popup>

4.配置文件

    pages/index/index.js文件里，增加

    option: {
      status: false,
      title: "购物车",
      height: 480
    }
    
# 配置

1.status

    status: 状态
    当为false时，关闭
    当为true时，打开
  
2.title

    title: 标题
    当title为undefined时，不显示标题

3.height

    height: 高度

    可选值为120，240，360，480

# 截图

![弹出框组件](http://cdn.tiantour.com/screenshot/popup.png)