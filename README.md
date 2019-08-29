# packerTool
安卓多渠道急速打包（packer-ng-plugin的java脚本打包实践）
## packer.bat
命令:java -jar packer-ng-v2-plus.jar --channels=channels_demo.json 
## 命令参数说明
java -jar packer-ng-v2-plus.jar jar执行命令
--channels= 因packer-ng-v2-plus.jar中写死就必须这样写
channels_demo.json 在config文件夹中要有这个json文件
## channels_demo.json 内容参数说明
 "sdkBuildToolsPath"：使用SDK的build-tools版本路径，使用时修改为自己as中使用路径和版本 eg："E:/Sdk/build-tools/29.0.2/"，29.0.2使用时改为as中的版本
"keystore"：包含path：jks的路径，storePassword密码，keyAlias别名，keyPassword密码
"packerQueue":包含release输入包和市场输出包键值对描述
## apk文件描述
cache：缓存可以不关注
original：放线上包，应用宝加固及360加固包。必须放名字要和config中的json文件originalApkName值相同
output：成功之后输出市场包路径


