### 项目结构

外面一层是内部类型

v1、v1beta1 这种是外部类型，validation 是用来验证内部类型的

conversion.go 是用来装换外部类型和内部类型，k8s 支持不同版本的互转，通过
内部版本可以减少这种装换函数


v1beta -> internal -> v1

default.go 是设置对象的默认值