# v0.0.2

## bug修正

+ 修正了无故增加`RPC`字段的bug

## 版本更新

+ grpc 1.38.0->1.43.0
+ spdloghelper@hsz/dev 0.0.1->0.0.2
+ schema_entry@hsz/dev 0.0.1->0.0.2
+ 使用的开发镜像更新至`alpine3.13-gcc10-conan1.44.0-protobuf3.17.1-grpc1.43.0`

## 新功能预备

+ 预备支持xds

# v0.0.1

目前只提供最基础的grpc服务端实现,并且只支持amd64平台

特性包括:

+ 使用conan管理依赖

+ grpc限定1.38.0版本

+ 建议在vscode中使用`dev_env.dockerfile`构造的容器中进行开发
