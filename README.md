## log-collect
    PHP+Swoole在作为网络通信框架上，对Phper有了一个过渡的选择；
    
    日志系统基于Swoole构建的常驻进程服务，利用Shell进行服务的基本管理，采用RabbitMQ队列来做对应的日志请求数据对接，基于Socket套接字进行数据通信；
     
    队列消费端采用多进程进行数据日志消费同步到RMS系统和日志数据归档；
    
    (原本二期计划是采用ELK进行对应数据呈现，时间问题项目搁置)。

## 后期计划
  - 日志落地，相关日志数据入到Elasticsearch搜索服务中，方面ELK对接以及相关日志查询；
  - 采用静态语言，诸如C、GO进行重构；
