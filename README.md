# CrawlWangYiMail
**1 使用需知**
- 使用selenium爬取网易邮箱内容需要解决html网页中iframe的定向问题，每次点击之后浏览器对象都要重新定位
- xpath语法也不是固定的，像网易邮箱这种网站过段时间都会重新进行维护，xpath定位有时是需要进行更新的
- 所需第三方库：selenium（自动化操作）、lxml（提供xpath语法）、pandas（保存数据）
- selenium所需浏览器：Microsoft Edge（默认），但需要提前安装对应驱动，点击这里查看[安装教程](https://blog.csdn.net/tk1023/article/details/109078613)

**2 爬虫思路**
- 首先使用selenium来模拟点击登录网易126邮箱
- 然后进入到收件箱的页面中，统计当前页面下有多少条订单数据
- 对这些订单邮件进行遍历操作，模拟点击每一封订单邮件
- 再进入邮件内部获取对应的表格数据，对这部分数据追加到初始化的列表中
- 最后使用pandas的DataFrame格式保存数据到csv文件中
- 
**3 你将会学到**
- [x] selenium软件的使用方法
- [x] lxml中xpath语法
- [x] Python中基础语法（循环和条件）

**4 其他**
- 代码开发者：欢迎点击我的[知乎首页](https://www.zhihu.com/people/zkl66)
- 如果想学习数据分析或者数据挖掘的，推荐查看我在[和鲸社区](https://www.heywhale.com/mw/project/61342a57c9c30f001878d043)上线的项目
