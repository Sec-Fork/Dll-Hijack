## Dll-Hijack

工具用于辅助白加黑免杀，之前提供的免杀模版已经不免杀废弃了。
用法：

```go
Usage: DllFuncexp.exe [OPTIONS]
Options:
  -f string
        DLL 文件名字
  -t string
        输出go源码类型或者cpp类型 (default "go")
exit status 1

```

成功会输出一个DLL.txt 文本
<img width="958" alt="image" src="https://user-images.githubusercontent.com/82130343/227850470-a02440e4-aea1-4ec1-bb24-118838cde7f7.png">

利用go的特性 只需要写出导出函数，利用init函数进行编写恶意代码，模版不提供。
<img width="943" alt="image" src="https://user-images.githubusercontent.com/82130343/227850570-3ba7a16e-b313-40e3-b025-2ad15caaf071.png">
写出DLL运行白加黑 就会优先加载init函数
<img width="202" alt="image" src="https://user-images.githubusercontent.com/82130343/227850679-466687a7-90f8-4261-9189-49ae6a8958d3.png">

c++ 由于不会，请自行探索。


## 免责声明
本工具仅面向合法授权的企业安全建设行为，如您需要测试本工具的可用性，请自行搭建靶机环境。

在使用本工具进行检测时，您应确保该行为符合当地的法律法规，并且已经取得了足够的授权。请勿对非授权目标进行扫描。

如您在使用本工具的过程中存在任何非法行为，您需自行承担相应后果，本人将不承担任何法律及连带责任。

在安装并使用本工具前，请您务必审慎阅读、充分理解各条款内容，限制、免责条款或者其他涉及您重大权益的条款可能会以加粗、加下划线等形式提示您重点注意。 除非您已充分阅读、完全理解并接受本协议所有条款，否则，请您不要安装并使用本工具。您的使用行为或者您以其他任何明示或者默示方式表示接受本协议的，即视为您已阅读并同意本协议的约束。
