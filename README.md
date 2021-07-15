# GeneralPay
通用支付

## gradle使用：

一、Project下的build.gradle文件下添加

allprojects {
    repositories {
      ...
      maven { url 'https://jitpack.io' }
    }
}

二、Module下的build.gradle文件下添加

dependencies {
          compile 'com.github.Lvluffy:GeneralPay:1.0.2'
}

或者

dependencies {
          implementation 'com.github.Lvluffy:GeneralPay:1.0.2'
}

其中包含微信支付三方包：com.tencent.mm.opensdk:wechat-sdk-android-without-mta:6.6.5
可使用剔除：
api ('com.github.gititcp:GeneralPay:1.0.2'){
   exclude group: 'com.tencent.mm.opensdk', module: 'com.tencent.mm.opensdk';
}

## 录屏
![xlu44-w3qwd](https://user-images.githubusercontent.com/34730376/56400355-150faf80-6286-11e9-82a9-21126cd509dc.gif)

