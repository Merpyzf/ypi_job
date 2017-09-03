Python模拟浏览器登录[天天爱学习] http://ypi.91job.gov.cn/ 获取积分，自动浏览题目，一个for循环搞定一切！
--
#### 看到这个文件则说明你们今天的积分已经领取过了，如果不放心的话可以亲自登录再查看一下当然不包括如下几位同学（31，41，47 好像是密码不正确）

实现大致流程：
--
1. 通过Chrome开发者工具分析用户登录的接口（http://ypi.91job.gov.cn/user/login?callback=login）
以及所需要提交的参数信息

![image](http://op225mmxn.bkt.clouddn.com/QQ20170904-010210@2x.png)

2. 登录成功后获取服务器返回的cookie,后续的操作将cookie提供给服务器就可以免登录了

3. 登录成功之后目的就达到了，当然为了做的更好一点，又加入了保存历史题目的功能，题目可以追加到文件当中去。

咳咳…… 敲黑板 如何使用？
--
1. 安装python2.7的版本(本机测试环境 2.7.10)
2. 使用到的第三方模块(BeautifuSoup4, requests),这两个模块需要额外安装,当然也很简单直接 pip install beautifulsoup4 就ok了，下一个同上，前提是有python的环境。
3. 下面直接运行就行了,命令:
```
python /Users/wangke/PycharmProjects/ypi_job/ypi_job_auto_login.py
```

### 测试的运行效果,一个for循环搞定全班同学的积分获取问题😄……

![image](http://op225mmxn.bkt.clouddn.com/yunxingxiaoguo%20.png)

😆😆😆

