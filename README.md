# Startblog

>一款基于Codeigniter、Amazeui开发的简洁、易用、跨平台自适应的Markdown博客系统.

>Author: [Cryin']

![](http://i1.piimg.com/567571/6947db2521f305f1.jpg)

###主页

 [http://cryin.startblog.cc/](http://cryin.startblog.cc/)

###程序功能：

>专业的markdown博文撰写、修改、删除功能,

>Markdown在线编辑器，实时预览;

>文章搜索、备份功能;

>站点、博文SEO信息设置;

>RSS订阅、友情链接功能;

###运行环境:
* php 5.x + mysql

###反馈:

本着大道至简的原则，本Blog程序只维持最基本的Blog形态，不会轻易增加其它功能。有任何问题可以反馈至issues或者qq交流。

###关于作者

* github https://github.com/Cryin

###贡献者

感谢辉哥设计的Logo，感谢贡献者LUHOO、Hardy、Ant、半城人、[Seven](http://www.sevenblog.cn/)

###捐赠者

感谢Hardy、gege的捐赠！

###安装方法:

>手动创建数据库

>将程序上传至站点根目录,输入http://www.yoursite.cc/install进行安装即可

如果安装在目录则根据站点目录

>修改application\config\config.php文件，添加目录字段，如目录为startblog：
$config['base_url'] = 'http://'.$_SERVER['SERVER_NAME'].'/startblog';

>修改.htaccess文件Rewrite规则，如目录为startblog则修改为：
>>RewriteEngine on  
>>RewriteCond $1 !^(index\.php|static|favicon\.ico|robots\.txt)  
>>RewriteRule ^(.*)$ /startblog/index.php/$1 [L]

###手动安装说明:

>根据站点目录设置application\config\config.php文件$config['base_url']项

>根据站点目录修改.htaccess文件Rewrite规则

>设置数据库配置信息：application\config\database.php文件

>创建数据库startblog，并导入sql文件，路径data\db\startblog.sql

>管理默认用户名、密码均为startblog


###Screenshot
后台文章管理:

![](http://i1.piimg.com/567571/6bbf83711d00c63b.png)

前台页面：

![](http://i1.piimg.com/567571/3ca2f44da1c73fea.png)

###更新说明:

>2014/9/18 初识CodeIgniter，编写博客程序！

>2015/3/27 实现markdown编辑器与解析

>2016/7/12 完成基本功能！version：startblog v1.0

>2016/7/22 初始化sql文件，修复xss问题及标签显示bug！

>2016/7/25 修改登录页面及标签页面！

>2016/7/27 完成站点SEO功能，增加url rewrite，完成文章页面seo功能，添加登录logo！version：startblog v1.1

>2016/7/27 增加about编辑功能，添加评论功能！version：startblog v1.2

>2016/8/1  增加rss订阅功能！version：startblog v1.3

>2016/8/5  增加install功能！version：startblog v1.4

>2016/10/23  修复markdown编辑器加载不稳定问题，修复post提交时bug！version：startblog v1.5

>2016/11/14  全面升级UI，采用Amazeui开发后台及前端UI！version：startblog v2.0

>2016/11/21  修改新建、编辑文章PV重置、数据库报错bug！version：startblog v2.0

>2016/11/25  新增友情链接编辑、排序功能，修改文件编辑界面，增加编辑框边框。修复dreamkill同学提出的bug及程序问题，输入输出统一进行安全过滤，model类修改为大写 ！version：startblog v2.1

>2016/12/02  修改新建文章时有时出现告警信息并暴露sql语句，增加文章配图随机功能，当封面配图为空时，随机显示图片 ！version：startblog v2.1

>2016/12/13  优化文章编辑界面,发布时间自动获取,添加新banner图，感谢辉哥制作！version：startblog v2.1
