### 检测网站广告是否被屏蔽

常用的屏蔽广告插件AdBlock、ADT广告终结者等，基本都是根据关键字来屏蔽广告js文件，比如cmp、adview、cpc等。

#### 检测方法
1. 创建一个名称含有广告关键字的JS文件，“adview_pic_guanggao_gg_ads.js”
2. JS文件内部创建一个变量，var adSkillTest = true;
3. 页面中引用这个JS文件，如果开启了广告屏蔽那么文件“adview_pic_guanggao_gg_ads.js”将不会被载入，也就是adSkillTest这个变量就不会存在
4. !adSkillTest 为真则说明开启了广告拦截并已经屏蔽了广告

