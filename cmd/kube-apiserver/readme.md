### apiServer

* 搞清楚有哪些启动参数可以配置
* ApiServer/ExtensionsServer 都是通过对应的配置初始化 server 的


* 通过版本实现兼容性，而不是改变数据结构，这样的好处是保证接口行为的一致性
* 通过 group 实现扩展 api

### CR 的扩展功能

* 通过 CRD
* Users needing the full set of Kubernetes API semantics can implement their own apiserver and use the aggregator to make it seamless for clients

* 通过设置 --runtime-config 可以开启和关闭一些 API GROUPS
* Enabling or disabling groups or resources requires restarting apiserver and controller-manager to pick up the --runtime-config changes