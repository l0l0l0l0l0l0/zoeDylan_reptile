>#爬虫

>爬虫就是虫,抓a标签的

>爬虫设置里面,选择器需要定位到a标签上面去 支持简单的层级选择 (>、+、~、:**)这些符号别来 要报错(#hot a)

>**自动缓存数据：db/reptile.data.json**

>**/admin**是管理界面

>**可以配置邮件**

>邮件发送人在管理界面里面去修改

>邮件接收人在管理界面里面可以直接配置

>可以直接**node server/reptile**直接启用爬虫

>也可以**node index**启用网站(默认爬虫也会同时启用)

>**server/reptile.js**里面有配置文件说明

>**配置文件别乱改,不然等着报错吧**

**2015-07-01 15:13:19**

>新增邮箱模版渲染功能,可以自己编辑模版,模版值有:网站名称(name)、描述(desc)、链接(url)和标题(title),

>>实例:

            <p>{{name}}</p>

**2015-07-01 17:02:47**

>取消了修改配置后提交未填帐号密码和邮箱密码会弹窗问题,现在修改后没填写密码默认使用之前的密码.

**2015-07-02 14:55:07**

>新增网页中的分类功能,不过现在仅限于网站分类,修复一个bug（爬的a标签的href属性是undefined会报错）