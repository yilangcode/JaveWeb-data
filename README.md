# JaveWeb-data
2022.4.5日结束的javaWeb学习的资源

## 采用了JavaEE的Dao、Service、Web三层架构
Dao只负责与数据库进行交互（从数据库连接池中取出连接）。Service层处理业务逻辑，Web层使用Servlet技术。
## 包含的技术点逻辑（由底层向上）
javaBean:编写客户、订单、商品等需要使用的javaBean对象
JDBCUtils： 构建服务器与数据库的连接
Dao层：获取连接，并执行最基本的查询语句
Service层：为Web层的业务逻辑提供具体的数据库查询服务
Web层：获取参数封装成javaBean对象，调用Service处理业务，进行重定向与转发
前端：以html为主体，域进行数据交换
## 小技术点
jsp抽取页面相同点
el表达式进行遍历，减少代码
cookie验证用户登录状态，session域处理购物车模块
filter执行拦截，配合threadlocal进行事务回滚；
json提供更高效的数据前后端交互
ajax提供局部异步的反馈，提供用户体验
