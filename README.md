# Dota2Work

模仿DotaMax的Dota2游戏助手，在登陆界面输入自己的steamID就能看到自己的比赛数据和数据分析。

数据源全部取自steam平台提供的dota2数据接口，没有自己搭建服务器后台，所以用户在运行的时候，进入个人战绩界面时，必须一次性获取完所有自己的比赛记录，否则将无法看到一些后续的数据。也因为如此，将会在本地储存几千条几万条的比赛数据，在运行的时候，都要对这些数据进行解析和分析，所以可能会有卡顿。
界面开发参考了许多大牛的界面，自己也模仿了一些view的开发。

主要的实现框架为：

网络框架：okhttp  

数据库保存：realm  

json解析：阿里fastjson  

图片加载：imageloader 

图表：MPAndroidChart

热修复：腾讯tinker   等等

英雄、物品详情界面：直接跳转dotamax的英雄界面，因为staam没有提供这方面的接口。

斗鱼直播：简单的调用了斗鱼api，用webview直接跳转到斗鱼界面

新闻：使用了百度开发平台中的新闻接口，就是信息量有点少。
