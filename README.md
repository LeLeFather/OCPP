# OCPP
OCCP Test Tools 
OCPP 是欧州地区的标准充电桩开发协议，其基于WEBSOCKET 传输模试，数据格式为JSON 格式。
本项目是基于上述协议开发的一个测试版本，方便开发人员要地测试应用。
本测试基于JDK1.8 以上版本开发，在运行前进安装好JDK环境。访问端口固定为8080
目录说明

config 配置文件
down 上传下载固件目录
start.bat 为运行目录 
ocppp_lib 为运行依赖包

正常运行后在控制台能看到这样的信息：
E:\oscp>java -jar ocpp.jar
log4j:ERROR Could not find value for key log4j.appender.error
log4j:ERROR Could not instantiate appender named "error".
2020-05-15 16:08:41,409 INFO [io.netty.handler.logging.LoggingHandler]:101 - [id
: 0xe9d54388] REGISTERED
2020-05-15 16:08:41,501 INFO [io.netty.handler.logging.LoggingHandler]:101 - [id
: 0xe9d54388] BIND(0.0.0.0/0.0.0.0:8080)
Open your web browser and navigate to http://127.0.0.1:8080/
2020-05-15 16:08:41,550 INFO [io.netty.handler.logging.LoggingHandler]:101 - [id
: 0xe9d54388, L:/0:0:0:0:0:0:0:0:8080] ACTIVE
最后通过路径：
http://127.0.0.1:8080/ocpp/user/user1  能访问到电桩主控测试页面。不成功一般都是JDK没按装正确，请确保JDK 正确安装


