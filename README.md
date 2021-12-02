# LiqunShield
蓝队工具箱

![image](https://user-images.githubusercontent.com/89302066/143564383-9891f196-ecbf-4cf9-8e6b-aa5dfb28778f.png)

下次更新剩余的Asp, Csharp, Php等未更新载荷解密以及 JavaAesRaw 载荷响应包的解密
更新完上述哥斯拉载荷解密后会更新shiro流量包解密以及新增webshell爆破功能

另外目前Base64版本的解密是可以直接从抓包工具（bp等）或者流量设备上的http请求获取, 进行url解码后即可通过该工具箱解密请求流量, 但是对于Raw版本的流量的解密, 目前的实现方式是通过wireshark等流量工具抓取16进制数据内容再放到该工具箱进行解密, 可这样总归有点限制, 正在思考如何有效通过抓包工具抓到的http请求来进行解密。

## 目前支持哥斯拉载荷的解密如下：
* CsharpAesBase64
* PhpEvalXorBase64（该载荷解密数据为key中的内容，而不是pass的，key中内容才是传输的加密内容）
* PhpXorBase64
* JavaAesBase64
* JavaAesRaw（该解密目前只支持请求包解密，且流量需要16进制数据，可通过wireshark抓取）等

JavaAesRaw 通过wireshark抓取到16进制流量解密如下：

![image](https://user-images.githubusercontent.com/89302066/144377113-ad2c700b-c2ad-4791-ab27-993ed91af7d8.png)

![image](https://user-images.githubusercontent.com/89302066/144377375-65fee1e3-3eef-4f65-8dcb-38a6db41f73b.png)



