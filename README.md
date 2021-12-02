# LiqunShield
蓝队工具箱

![image](https://user-images.githubusercontent.com/89302066/143564383-9891f196-ecbf-4cf9-8e6b-aa5dfb28778f.png)

## 目前支持哥斯拉载荷的解密如下：
* CsharpAesBase64
* PhpEvalXorBase64（该载荷解密数据为key中的内容，而不是pass的，key中内容才是传输的加密内容）
* PhpXorBase64
* JavaAesBase64
* JavaAesRaw（该解密目前只支持请求包解密，且流量需要16进制数据，可通过wireshark抓取）等
