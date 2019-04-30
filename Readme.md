原地址 https://www.evernote.com/l/AXZBLcz_u_1Fs6Ju7yvdGAuJMMNcrJwrLCs


1. 设计优先
    1. 极简原则 （不是粗暴简单，而是设计时候尽量检查减少依赖）
2. 底层驱动，
    1. models 编写！测试用例 尽量保证没有依赖
    2. services编写！测试用例 包含一些列功能！需要编写测试用例覆盖
    3. API编写！ 测试用例 包含模拟的正常用户需求
3.  架构之开发效率
    1.  路由
    2. 参数检验
    3. 依赖注入，容器
    4. 分层 services / model
    5. cache
    6.  Log (input/output | DB | dubug error | other log)
    7. model (事物，基础CURD)
    8. Exception Catch
    9.  Third Library
    10. Hook (function / event )
    11. Queue
    12. Crontab Script
    13. Yourself Common Library
    14.  CodeCeption Or PhpUnit ( model /service / api ) 简称单元测试 功能测试 集成功能测试
    15. CI   自动化测试 目前还是比较简单的命令行跑 需要进一步学习
4. 业务篇
    1. 短信
    2. 支付
    3. User Message
    4. Push Message
    5. 账户数值
        1. Wallet 钱包
        2. Credit 积分
        3. Coin 金币
        4. 其他等等
    6. DB Table Log篇 
        1. Operation 操作日志
        2. Status change 日志
    7. 账号授权+鉴权
    8. 单点登录 SSO
    9. Oauth2 授权
    10. 文件上传 OSS 七牛
        1. file type 
            1. Image  
            2. Video 
            3. Pdf / doc / Excel
    11. 核心业务  
    12. 其他业务（一次性业务，运营相关，只要不是核心业务，无论优先级如何，切记代码非侵入式）
        1. 例如，一次活动中需要给用户加金币
            1. 活动逻辑由活动模块控制
            2. 加金币操作其实是核心业务之一，直接调用核心业务金币组件的方法
            3. 其他情况类似！
5. 进阶篇
    1. DB安全
        1. 索引
        2. Uniqe 索引
        3. 锁（乐观锁+事物锁）
    2. 代码质量
        1. 单元测试  针对db model 
        2. 功能测试  针对service 
        3. Api 测试   针对API 模拟curl 
    3. 配置中心
        1. development 开发环境
        2. debug 测试环境
        3. production 生产环境
    4. 自动化
        1. 代码自动发布
        2. 文档自动生成
        3. 报错日志自动化
    5. Nginx Mysql PHP 日志
        1. ELK 
6. 高级篇
    1. Docker. Vagrant K8s
    2. RPC  
    3. Swoole
        1. 作为http服务器
        2. 作为TCP服务器
        3. 作为UDP服务器
        4. 作为socket服务器
        5. 作为crontab 毫秒级任务
    4. Consol / ACM阿里云 云端配置中心
    5. 存储集群
        1. DB 集群
        2. Cache 集群
        3. File 集群
    6. ELK
    7. Zookeeper 
7. 前端
    1. 每个phper多少需要懂得一些前端知识
    2. 框架VUE react angular 
    3. Nodejs编程思想
