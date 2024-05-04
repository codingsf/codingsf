#### 一、概述
微信客户端小程序抓包

#### 二、校验
##### 1、vx版本：3.9.7.29
##### 2、特征定位
模块名：wechatwin.dll
关键字符串：ida打开wechatwin.dll， 然后搜索特征字符串“AppletHostWrapper::JsApiHandlerCallback api_name=%s” 交叉引用看下那个函数，5个参数。
##### 3、frida WeChat.exe -l hook.js