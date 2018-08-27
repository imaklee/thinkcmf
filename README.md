ThinkCMF 5.0.180901 开发版
===============

### 系列讲座
https://www.thinkcmf.com/college.html

### ThinkCMF5主要特性
* 基于全新 ThinkPHP5.0开发
* 更规范的代码,遵循PSR-2命名规范和PSR-4自动加载规范
* 更规范的数据库设计
* 前后台完全基于bootstrap3
* 增加 api 模块（需单独下载）
* 支持 composer 管理第三方库
* 核心化：独立核心代码包
* 应用化：开发者以应用的形式增加项目模模块
* 插件化：更强的插件机制，开发者以插件形式扩展功能
* 模板化：模板完全傻瓜式，用户无须改动任何代码即可在后台完成模板设计和配置
* 增加 URL美化功能，支持别名设置，更简单
* 独立的回收站功能，可以管理所有应用临时删除的数据
* 统一的资源管理，相同文件只保存一份
* 注解式的后台菜单管理功能，方便开发者代码管理后台菜单
* 文件存储插件化，默认支持七牛文件存储插件
* 模板制作标签化，内置多个cmf标签，方便小白用户
* 更人性化的导航标签，可以随意定制 html 结构
* 后台首页插件化，用户可以定制的网站后台首页

### 环境推荐
> php5.5+

> mysql 5.6+

> 打开rewrite


### 最低环境要求
> php5.4+

> mysql 5.5+ (mysql5.1安装时选择utf8编码，不支持表情符)

> 打开rewrite


### 运行环境配置教程
https://www.thinkcmf.com/topic/1502.html


### 自动安装
> 之前安装过 cmf5的同学,请手动创建`data/install.lock`文件

代码已经加入自动安装程序,如果你在安装中有任何问题请提交 issue!

1. public目录做为网站根目录,入口文件在 public/index.php
2. 配置好网站，请访问http://你的域名

enjoy your cmf~!

### 系统更新
如果您是已经安装过 cmf5的用户,请查看 update 目录下的 sql 升级文件,根据自己的下载的程序版本进行更新

### API开发 (支持app,小程序,web)
如果你需要 `api` 开发请下载:  
ThinkCMF5 API :https://github.com/thinkcmf/thinkcmfapi

### 完整版目录结构
```
thinkcmf  根目录
├─api                   api目录(核心版不带)
├─app                   应用目录
│  ├─portal             门户应用目录
│  │  ├─config.php      应用配置文件
│  │  ├─common.php      模块函数文件
│  │  ├─controller      控制器目录
│  │  ├─model           模型目录
│  │  └─ ...            更多类库目录
│  ├─ ...               更多应用
│  ├─command.php        命令行工具配置文件
│  ├─common.php         应用公共(函数)文件
│  ├─config.php         应用(公共)配置文件
│  ├─database.php       数据库配置文件
│  ├─tags.php           应用行为扩展定义文件
│  └─route.php          路由配置文件
├─data                  数据目录
│  ├─conf               动态配置目录
│  ├─runtime            应用的运行时目录（可写）
│  └─ ...               更多
├─public                WEB 部署目录（对外访问目录）
│  ├─api                api入口目录(核心版不带)
│  ├─plugins            插件目录
│  ├─static             静态资源存放目录(css,js,image)
│  ├─themes             前后台主题目录
│  │  ├─admin_simpleboot3  后台默认主题
│  │  └─simpleboot3            前台默认主题
│  ├─upload             文件上传目录
│  ├─index.php          入口文件
│  ├─robots.txt         爬虫协议文件
│  ├─router.php         快速测试文件
│  └─.htaccess          apache重写文件
├─simplewind         
│  ├─cmf                CMF核心库目录
│  ├─extend             扩展类库目录
│  ├─thinkphp           thinkphp目录
│  └─vendor             第三方类库目录（Composer）
├─composer.json         composer 定义文件
├─LICENSE.txt           授权说明文件
├─README.md             README 文件
├─think                 命令行入口文件
```

### 开发手册
http://www.kancloud.cn/thinkcmf/doc

### QQ群:
`ThinkCMF 官方交流群`:316669417  
   
`ThinkCMF 高级交流群`:100828313 (付费)  
高级群专属权益:  
第一波:两个后台风格(ThinkCMF官网风格后台主题,蓝色风格后台主题)  
第二波:ThinkCMF5完全开发手册离线版(PDF,EPUB,MOBI格式)  
更多专属权益正在路上...

`ThinkCMF 铲屎官交流群`:415136742 (生活娱乐，为有喵的猿人准备)

### 话题专区
http://www.thinkcmf.com/topic/index/index/cat/11.html

### 反馈问题
https://github.com/thinkcmf/thinkcmf/issues

### 更新日志
#### 5.0.180901
* 增强模板设计，提供可视化模板设计
* 增加模板设计界面钩子
* 增加验证码图片钩子
* 增加后台设置网站信息界面钩子
* 增加后台清除缓存界面钩子
* 增加后台导航管理界面钩子
* 增加后台友情链接管理界面钩子
* 增加后台幻灯片管理界面钩子
* 增加后台管理员列表界面钩子
* 增加后台角色管理界面钩子
* 增加用户管理本站用户列表界面钩子
* 增加资源管理列表界面钩子
* 增加用户管理第三方用户列表界面钩子
* 增加后台首页界面钩子
* 增加后台回收站界面钩子
* 增加后台菜单管理界面钩子
* 增加admin.js`js-ajax-btn`组件 
* 优化插件加载
* 优化前后台上传js


[门户应用]
* 增加文章音频，视频功能
* 增加门户后台文章管理列表界面钩子
* 增加门户后台文章分类管理列表界面钩子
* 增加门户后台页面管理列表界面钩子
* 增加门户后台文章标签管理列表界面钩子

#### 5.0.180626
* 升级TP到`5.0.20`
* 增加插件REST api基类`PluginRestBaseController`
* 增加我的喜欢功能
* 增加手机相关设备类型判断函数
* 优化百度编辑器视频上传
* 优化get_client_ip()方法，默认使用高级模式
* 优化手机号检查支持国际手机号
* 优化图片和文件链接转化函数
* Restful api基类增加apiVersion属性
* 修复邮箱验证码发送失败
* 七牛插件增加东南亚节点
* 前台模板文件解析标准化

[门户应用]
* 增加文章`thumbnail`字段
* 增加文章收藏数功能

#### 5.0.180525
* 修复ajax请求普通页面时返回格式为json
* 优化图片链接生成
* 修复插件模板常量地址问题
* 修复后台用户注册验证开关错误 #481
* 增加后台刷新后保持当前页面的功能 #475
* 取消用户名注册和绑定功能
* 优化无限滚动jquery插件

#### 5.0.180508
* 修复用户注册问题
* 优化缓存清理，防止删除日志文件

#### 5.0.180501
[核心]
* 升级TP到5.0.19，增强安全性
* 修复模板设计数组编辑验证规则不生效 #440
* 修复后台登录失效后iframe里加载首页
* 修复七牛插件上传云存储文件没有后缀名问题#437
* 修复删除评论时的错误文案提示 #443
* 修复ueditor漏洞#431
* 修复PHP7.2下后台清除报错
* 修复前台账号绑定无法获取mobile、email验证码 #418
* 修复百度编辑器大附件上传问题
* 修复百度编辑器大视频文件上传问题
* 升级font awesome到4.7.0

[门户应用]
* 修复文章分类修改层级后子分类层级不更新问题
* 优化 portal:articles 标签field,order 属性支持 php 变量
* 修复文章分类别名设置为纯数字，路由生成错误，无法访问。 #438
* 增加页面相册和附件功能 #449

#### 5.0.180123
[核心]
* 增加小程序管理插件
* 增加插件后台首页左侧菜单显示 
* 增加 themes 根命名空间
* 增加模板设计图片模板变量取消功能
* 增加插件自定义处理配置功能
* 增加插件后台权限管理功能
* 增加后台模板切换
* 增加直传云存储功能
* 增强导航和子导航标签，自定义更随意
* 增加before_content,fetch_upload_view,log_write_done,switch_admin_theme钩子
* 增加PluginAdminBaseController基类
* 增加系统钩子同步
* 增加插件中可使用$site_info变量
* 增加 xml 生成函数
* 增加插件设置上传文件组件
* 优化数字验证码日志写入增加过期时间配置
* 优化数字验证码逻辑，增加数字验证码发送图片验证码,【升级时注意界面逻辑】
* 优化验证码生成功能，可增加验证码插件管理验证码生成
* 优化钩子插件管理
* 优化插件注册机制 
* 优化后台首页菜单加载
* 修复模板管理变量数据为array时删除出错 #392
* 修复后台管理搜索翻页时条件丢失问题 #366
* 修复删除第三方用户时报错 #368
* 修复在使用cdn加速js时后台文章编辑器时无法加载编辑器配置
* 修复模板设计模板变量file类型不支持上传 #136
* 修复用户行为周期设置无效 #382
* 修复个人信息编辑签名验证问题
* 修复用户生日早于1970年报错
* 修复地址坐标选择搜索后无法确定坐标问题
* 优化IE8,9下的兼容问题
* 优化前台未登录时跳转方式

[安装程序]
* 增加安装时管理员密码长度限制 #334 
* 增加安装时检查 rewrite设置
* 增加安装时 innodb 检测
* 更正PHP版本要求

[门户应用]
* 优化portal:articles标签可在模板里设置分页参数和样式
* 优化portal:articles标签所有属性都支持PHP变量
* 优化标签控制器支持标签名
* 增加portal:tagArticles标签
* 取消文章列表用户关联查询
* 修复文章多分类进文章列表文章重复问题


#### 5.0.170927
[核心]
* 增加是否开放注册设置
* 增加已经安装模板文件检测是否已经删除功能
* 增加模板卸载风险提示
* 增加钩子同步功能
* 增加用户操作同步功能 #291
* 增加网站信息【$site_info】变量，可以在插件中使用 #310
* 修复添加管理员不能登录 #110
* 优化 admin.js
* 优化后台模板设计排版
* 优化后台加密码设置
* 返回按钮统一优化
* 优化 url 美化时规划选择
* 修复`api`模块缺少函数报错
* 修复回收站还原提示错误 #111
* 修复原始网址和显示网址同时有参数的情况下，两个参数值相同的时候不能解析URL
* 修复模板设计数组编辑功能缺失
* 修复后台登录在双核浏览器下会使用 IE 内核问题#168
* 修复模板widget只有数组时，后台设计保存时报错
* 修复日期选择在windows firefox下报错
* 修复模板设计数据源页面清空链接错误
* 修复后台模板设计，json文件中的数组数据，不能正常显示 #222
* 修复`cmf\lib\Auth\check`方法逻辑问题 #252
* 修复后台用户登录自动退出后iframe页跳转到首页的问题
* 修复用户个人资料修改问题
* 修复绑定手机号和绑定邮箱号惟一性提示信息错

[安装程序]
* 更改安装时数据库默认为127.0.0.1
* 优化安装时链接生成

[门户应用]
* 增加前台文章控制器默认分类指定
* 增加后台文章列表所在分类列
* 增加后台文章分类必须指定分类验证
* 增加 portal:articles 标签 limit可以设置变量
* 增加模板设计页面数据源
* 完善 ApiService获取指定分类下的所有子分类方法
* 增加portal:categories,portal:subCategories,portal:allSubCategories标签
* 增加文章、页面、分类模板选择时模板文件名称查看
* 增加文章保存钩子
* 优化指定分类下所有子分类获取方法
* 修复文章分类管理中不保存选择的模板 #107
* 修复面包屑标签 self属性无法识别 false
* 修复后台编辑文件会覆盖原作者ID #175
* 修复后台文章保存后排序变化问题
* 修复添加文章分类时 path 没数据问题

[升级指导]
https://www.kancloud.cn/thinkcmf/doc/327443

#### 5.0.170607
[核心]
* 删除 app/common.php
* 规范 admin.js frontend.js函数名
* 更改后台模板设计的模板文件列表排序规则为从小到大排序
* 增加模板切换钩子，方便开发者实现复杂的模板切换功能
* 增加插件作者和演示信息
* 增加数字验证码模板编辑功能
* 增加模板变量编辑控件color
* 增加插件配置组件时间，图片，地理位置，颜色
* 优化模板配置更新
* 优化文件上传，检查已经上传文件是否存在，不存在重新上传
* 修复插件增加新配置时报错
* 修复模板变量 rule 规则存在，但没有规则时模板设计保存会报错
* 修复后台清除缓存后url生成不美化
* 修复模板设计一个页面有多个数组编辑问题
* 修复cdn设置不生效
* 修复后台菜单添加子菜单不选择上级问题
* 修复后台可能多个滚动条
* 修复后台添加、编辑角色一处文字错误
* 修复插件更新时不更新新增的钩子

[门户应用]
* 完善前台模板钩子
* 完善文章标签功能
* 增加前台模板手机注册关闭开关
* 优化文章后台文章分类链接生成
* 修复ff下文章相册图片替换和删除问题
* 修复文章分类排序功能

#### 5.0.170520
[核心]
* 完善插件后台管理
* 后台登录插件化
* 后台首页插件化
* 文件存储插件化
* 增加 URL 美化功能
* 增加后台加密码功能
* 增加用户修改头像
* 增加插件设置表单验证
* 增加前台后台通用语言包
* 增加编辑器里上传文件链接替换
* 增加应用 command.php 配置文件
* 增加后台管理员添加编辑用户名，邮箱惟一性验证
* 优化安装程序
* 优化上传文件
* 优化后台首页
* 优化回收站
* 优化插件启用禁用
* 优化小屏下后台首页不兼容问题
* 优化后台图片查看
* 修复后台菜单编辑不生效
* 修复幻灯片添加不显示问题
* 修复导航数据源数据返回为空时报错
* 修复 pathinfo 模式下后台本站用户默认头像不显示问题
* 修复后台 cdn 不能设置
* 合并asset应用到 user

[门户应用]
* 增加文章收藏功能
* 增加文章点赞限制,一个用户只能点赞一次
* 增加文章分类缩略图
* 优化文章分类管理删除
* 优化文章页和页面页内容图片样式问题
* 修复文章添加编辑默认图片错误
* 修复分类下没有文章时报错
* 修复页面模板设置无效
* 修复页面删除后仍可以访问

#### 5.0.170505
[核心]
* 完善用户注册流程
* 完善插件功能
* 增加手机验证码发送钩子
* 增加手机验证码发送演示插件
* 增加用户邮箱绑定
* 增加用户手机绑定
* 增加常用模板钩子
* 增加模板设计图片上传
* 增加用户密码修改
* 增加用户收藏功能
* 增加导航标签,子导航标签增加 `max-level` 设置
* 修复邮箱验证码发送
* 修复windows下获取模板数据时模板文件路径问题
* 修复单文件,多文件上传
* 修复后台首页用户昵称一直显示admin
* 修复 `navigation`,`subNavigation` 标签两个以上不能同时使用问题
* 修复 console 模式报错
* 取消前台有错误时界面刷新

[门户应用]
* 增加文章附件功能
* 优化文章相册

#### 5.0.170422
[核心]
* 完善幻灯片
* 完善后台控制器方法注释
* 增加调试模式下实时更新模板配置
* 增加友情链接图片上传
* 增加应用公共语言包功能
* 增加资源管理
* 增加模板设计数据源层级关系
* 更新jQuery Form版本
* 增加后台菜单类型是否有界面区分
* 增加权限验证时权限规则里没有的规则不用验证
* 增加前台网站信息获取
* 优化后台菜单导入
* 统一排序规则,按从小到大排序
* 修复后台模板管理点更新提示卸载
* 修复标签`NavigationMenu`
* 修复菜单导入时未添加权限规则
* 修复`navigationFolder`设置多个子菜单后会多循环数据
* 修复部分代码php5.4下不兼容
* 修复后台菜单不能添加编辑

[门户应用]
* 完全独立门户应用
* 完善后台页面管理
* 完善面包屑标签`breadcrumb`
* 完善文章分类管理
* 完善文章管理
* 修复文章分类`path`更新
* 优化文章列表标签`articles`
* 优化后台文章分类选择
* 增加前台文章点赞功能
* 增加前台文章搜索功能
* 增加文章列表分页总数获取

#### 5.0.170401
* 完善文件上传
* 增加回收站功能
* 完善友情链接
* 优化网站设置
* 增加后台登陆验证码
* 修复后台用户密码修改
* 修复用户管理-本站用户头像不显示
* 完善前台用户登录注册
* 增加后台菜单导入
* 修复后台菜单列表排序
* 完善导航
* 增加插件钩子管理
* 完善前台模板


