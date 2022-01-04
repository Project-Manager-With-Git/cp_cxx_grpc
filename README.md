# cp_cxx_grpc

C++语言grpc项目的组件仓库

目前只提供最基础的grpc服务端实现,并且只支持amd64平台

特性包括:

+ 使用conan管理依赖

+ protobuf限定1.17.0版本
+ grpc限定1.43.0版本

+ 建议在vscode中使用`dev_env.dockerfile`构造的容器中进行开发

编译grpc文件,两种方式:

1. `ppm grpc build -t src -i pbschema <pbfilename>`
2. `protoc  -I /workspaces/testcxxgrpc/pbschema -I /workspaces/testcxxgrpc/pbschema  --grpc_out=src/<pbfilename>_pb --plugin=protoc-gen-grpc=/root/.conan/data/grpc/1.43.0/_/_/package/5ec89ccf231731cfeb7c8350d629717adf8eb6dd/bin/grpc_cpp_plugin --cpp_out=src/<pbfilename>_pb <pbfilename>`