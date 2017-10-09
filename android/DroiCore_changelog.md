# 更新日志

## Android Core-SDK v1.1.4035 `(2017-9-28)`  
```  
1. DroiUser新增OTP登录同步方法和获取session有效时间方法  
2. OTP登录异步方法增加boolean返回值  
3. 第三方登录增加获取和检测OAuthKey方法  
4. 修复已知bug  
```     

## Android Core-SDK v1.1.4014 `(2017-9-7)`  
```  
1. 移除DroiCloud的自动登录操作  
2. 优化代码  
```     

## Android Core-SDK v1.1.4006 `(2017-8-31)`  
```  
1. 完善权限不足时查询DroiReference返回结果  
2. DroiFile增加触发匿名登录动作  
3. 优化代码  
```     

## Android Core-SDK v1.1.3966 `(2017-8-17)`  
```  
1、增加对部分手机的兼容  
2、优化部分代码逻辑
```   

## Android Core-SDK v1.1.3965 `(2017-8-10)`  
```  
1、修复OkHttp版本低可能引发错误问题  
2、优化日活统计逻辑；
```   

## Android Core-SDK v1.1.3943 `(2017-7-27)`  
```  
1、优化代码逻辑和程序性能  
```   

## Android Core-SDK v1.1.3917 `(2017-7-20)`  
```  
1、修复 DroiFile getUri 失败情况下会传回正确DroiError问题  
2、修复未登录时調用 DroiUser.saveInBackground执行回调失败问题  
3、移除对 DroiAccount OAuth 支持  
```   

## Android Core-SDK v1.1.3893 `(2017-7-6)`  
```  
1、本版本开始要求OkHttp3更新到3.8.0(含)以上
2、修复DroiCloud.callRestApi GET参数非null无提示问题  
3、支持在ArrayList上设置@DroiReference  
4、支持DroiOAuthProvider构建传入Scope  
5、支持微信登录后获取AccessToken和OpenId  
```  

## Android Core-SDK v1.1.3854 `(2017-6-22)`  
```  
1、修复loginOTP返回DroiError错误问题  
2、修复安全性问题  
```  

## Android Core-SDK v1.1.3727 `(2017-5-23)`
```
1、修复 DroiObject.saveEventualy 无法使用的问题
2、去除 DroiPreference.getJsonObject
3、新增 DroiUser.resetPassword type - EMAIL&ALL
4、修复 DroiFile in DroiReference 的问题
5、新增文件大小为0时，DroiFile.save 会报错
6、更改 DroiReferenceObject.droiObject type 为 DroiObject*
```

## Android Core-SDK v1.1.3727 `(2017-5-9)`
```
1、修复注册后，isAnonymous仍是True的问题
2、新增DroiError.NATIVE_LIBRARY_NOT_FOUND
3、新增DroiError.getTicket
4、新增返回错误，当DroiCloud.callResetApi "GET"/"DELETE"的传入参数不为null
5、新增DroiObject.atomicAdd api
6、修复由于 QQ/Weixin SDK 更新，第三方授权无法使用的问题
7、修复DroiFile save progress
8、修复List<DroiFile> 无法 DroiQuery 回来的问题
```  

## Android Core-SDK v1.1.3676 `(2017-4-14)`
```
1、修复condition.isNull 报exception的问题
2、新增DroiUser.isEnabled API
3、修复Core.initialize ANR的问题
4、修复DroiUser.changePassword回传1040010，改成1070003
5、新增DroiFile.hasUri
6、新增DroiFile的uri会在上传后缓存
7、修复手机时间修改正确后，还是回传1070201的问题
```  

## Android Core-SDK v1.1.3652 `(2017-3-24)`
```
1、更新 DroiFile v2（七牛）
2、修复 index out of bound exception 问题
```  

## Android Core-SDK v1.1.3573 `(2017-3-16)`
```
1、调整signup流程，注册一般用户失败不会留下一个匿名用户
2、新增注册用户已存在时，会回传 DroiError.USER_ALREADY_EXISTS
3、新增DroiUser.resetPassword和DroiUser.confirmResetPassword
4、修复isnull/isnotnull无效的问题
5、新增海外导流机制（iplist v2）
```  

## Android Core-SDK v1.0.3512 `(2017-1-13)`
```
1、修复DroiGroup.fetchRelation结果为空的问题
2、修复保存List<String>到localstorage出错的问题
3、新增DroiCloud.callRestApi方法调用cloud code 
```  

## Android Core-SDK v1.0.3466 `(2016-12-29)`
```
1、修复使用Intent传输 droiobject时产生exception的问题
2、新增检查DroiFile缓存的md5
```  

## Android Core-SDK v1.0.3454 `(2016-12-21)`
```
功能更新：  
1、修复已知bug
2、新增DroiCondition.selectIn 支持 List
3、去除 DroiFile 最大大小限制，改为在服务端检查
```  

## Android Core-SDK v1.0.3449 `(2016-11-24)`
```
功能更新：  
1、修复已知bug
2、DroiUser缓存优化
```  

## Android Core-SDK v1.0.3428 `(2016-11-10)`
```
功能更新：  
1、修复已知bug
2、优化初始化流程，减少网络连接次数
```  

## Android Core-SDK v1.0.3378 `(2016-10-28)`
```
功能更新：  
1、修复 DroiUser 相关bug
2、增加 DroiFile.getSize & DrioFile.getMd5 方法
```  

## Android Core-SDK v1.0.3350  `(2016-10-22)`
```
功能更新：  
1、发布正式版本
2、修复已知 bug
3、增加部分 error 信息log
```
