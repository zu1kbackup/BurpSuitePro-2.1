## BurpSuitePro-2020.11.3

> **破解BurpSuitePro-2020.11.3版本**

- **[2020.1 - ~ 通杀loader来自x-Ai](https://github.com/x-Ai/BurpSuiteLoader)**

**据官方消息，官方对网站进行了调整，且故意开放了各系统的下载接口**

**下载方式**

```
https://portswigger.net/burp/releases/download?product=pro&version=2020.11.3&type=jar

https://portswigger.net/burp/releases/download?product=pro&version=2020.11.3&type=windowsx64

https://portswigger.net/burp/releases/download?product=pro&version=2020.11.3&type=macosx

https://portswigger.net/burp/releases/download?product=pro&version=2020.11.3&type=linux
```

**不但新版可以下载，旧版本也可以！！！**

> **SHA256 && MD5**

- **burp-keygen-scz**
- - **SHA256: 74893842a782238f52f0f225c06fa744568321911fea077bc290bd9914b73402**
- - **MD5: e646b3eef03efba637e6ed794ced4114**

- **burp-loader-x-Ai**
- - **SHA256: 1e54fbbaf3423c8b15b2507cb1e8c18092b0f728aa705ef8d235ac4300cd3e29**
- - **MD5: defafc938a0344b188d7273d3dd3eb48**

> **Win使用**

*一、初次使用*

  ```
  0x00 - 配置好java环境，Java9-Java14
  0x01 - 启动 burp-keygen-scz.jar，用来破解license
  Powershell：java -jar "C:\Users\User\Desktop\burp-keygen-scz.jar"

  0x02 - 加载 burp-loader-x-Ai.jar 启动 burpsuite_pro_v2020.11.3.jar
  Powershell：java -noverify -javaagent:"C:\Users\User\Desktop\burp-loader-x-Ai.jar" -Xmx2048m -jar "C:\Users\User\Desktop\burpsuite_pro_v2020.11.3.jar"

  0x03 - BurpSuite界面取消协助，同意协议
  0x04 - 随意修改 burp-keygen-scz 的 License Text
  0x05 - 把 License 复制到 BurpSuite
  0x06 - 点击 Manual activation，点击 Copy request
  0x07 - 把 Request 复制到 burp-keygen-scz 的 Activation Request
  0x08 - 把自动生成的 Activation Response 复制回 BurpSuite
  0x09 - 完成，开始使用
  0x10 - 持久启动必须加载 burp-loader-x-Ai.jar，不然依旧要license key
  ```

*二、使用过bp，已激活过license*

  ```
  0x01 - 直接加载 burp-loader-x-Ai.jar 启动 burpsuite_pro_v2020.11.3.jar
  Powershell：java -noverify -javaagent:"C:\Users\User\Desktop\burp-loader-x-Ai.jar" -Xmx2048m -jar "C:\Users\User\Desktop\burpsuite_pro_v2020.11.3.jar"
  ```

**bat_script**

 ```powershell
 @echo off 
 if "%1" == "h" goto begin 
 mshta vbscript:createobject("wscript.shell").run("%~nx0 h",0)(window.close)&&exit 
 :begin
 
 "C:\Program Files (x86)\Common Files\Oracle\Java\javapath\java.exe" -noverify -javaagent:"C:\Users\User\Desktop\burp-loader-x-Ai.jar" -Xmx2048m -jar "C:\Users\User\Desktop\burpsuite_pro_v2020.11.3.jar"
 ```

**TLS1.3和ipv4的问题**

- `-Djava.net.preferIPv4Stack=true`

> **Linux使用**

*一、初次使用*

  ```
  0x00 - 配置好java环境，Java9-Java14
  0x01 - 启动 burp-keygen-scz.jar，用来破解license
  /usr/lib/jvm/java-14-openjdk-amd64/bin/java -jar /opt/BurpSuite/burp-keygen-scz.jar

  0x02 - 加载 burp-loader-x-Ai.jar 启动 burpsuite_pro_v2020.11.3.jar
  /usr/lib/jvm/java-14-openjdk-amd64/bin/java -Dfile.encoding=utf-8 -noverify -javaagent:/opt/BurpSuite/burp-loader-x-Ai.jar -Xmx2048m -jar /opt/BurpSuite/burpsuite_pro_v2020.11.3.jar

  0x03 - BurpSuite界面取消协助，同意协议
  0x04 - 随意修改 burp-keygen-scz 的 License Text
  0x05 - 把 License 复制到 BurpSuite
  0x06 - 点击 Manual activation，点击 Copy request
  0x07 - 把 Request 复制到 burp-keygen-scz 的 Activation Request
  0x08 - 把自动生成的 Activation Response 复制回 BurpSuite
  0x09 - 完成，开始使用
  0x10 - 持久启动必须加载 burp-loader-x-Ai.jar，不然依旧要license key
  0x11 - 可以写个执行的shell，扔到/usr/bin下面
  ```

*二、使用过bp，已激活过license*

  ```
  0x01 - 直接加载 burp-loader-x-Ai.jar 启动 burpsuite_pro_v2020.11.3.jar
  /usr/lib/jvm/java-14-openjdk-amd64/bin/java -Dfile.encoding=utf-8 -noverify -javaagent:/opt/BurpSuite/burp-loader-x-Ai.jar -Xmx2048m -jar /opt/BurpSuite/burpsuite_pro_v2020.11.3.jar
  ```

> Usage:

*[!]- First use Burpsuite*

- **0x01. `burp-loader-x-Ai.jar` only the function of starting burpsuite, cracking license must use `burp-keygen-scz.jar`**
- **0x02. configure Java environment, Java9 - Java14**
- **0x03. start-up `burp-keygen-scz.jar` to crack license**
- - `java -jar "C:\Users\User\Desktop\burp-keygen-scz.jar"`
- **0x04. open burp**
- - `java -noverify -javaagent:"C:\Users\User\Desktop\burp-loader-x-Ai.jar" -Xmx2048m -jar "C:\Users\User\Desktop\burpsuite_pro_v2020.11.3.jar"`
- **0x05. `burpsuite` window, `cancel help` , `consent agreement`**
- **0x06. switch to `burp-keygen-scz.jar` window, modify at will `License Text`**
- **0x07. copy the `License` to burpsuite**
- **0x08. click `Manual activation`, copy `request` to `burp-keygen-scz.jar` 's `Activation request`**
- **0x09. copy the automatically generated `Activation Response` back to burpsuite**
- **0x10. finish, enjoy**
- **0x11. [!] the `burp-loader-x-Ai.jar` must be loaded before persistent startup, or license is still required**

*[!]- if u've cracked the license*

- **0x01. open burp**
- - `java -noverify -javaagent:"C:\Users\User\Desktop\burp-loader-x-Ai.jar" -Xmx2048m -jar "C:\Users\User\Desktop\burpsuite_pro_v2020.11.3.jar"`

> **依旧坚持更新的大佬们**

- [1. 目前可用的通杀loader from x-Ai](https://github.com/x-Ai/BurpSuiteLoader)

- [2. 四哥Blog](http://scz.617.cn:8/misc/201910151519.txt)

- [3. @nszy007]()

- [4. 微信公众号: 信安前线]()

- [5. 法海之路](https://www.fahai.org/)

- [6. Mrxn's Blog](https://mrxn.net/)

- [7. 小晨曦](https://xcxmiku.com/)

> **致敬**

- [1. 四哥Blog](http://scz.617.cn:8/misc/201910151519.txt)

- [2. 四哥微信公众号: 青衣十三楼飞花堂]()

> **某个可以第一时间更新pro jar包的网站(但多数收费)**

- [Raidforums](https://raidforums.com/Forum-Cracking-Tools)

> **破解**

```
Java 9至13，可以用javaagent的方式patch，这种在8上也能用。
Java 9至13，还可以用patch-module的方式，但8不能用。
如果Burp Pro不换注册机制，可以一直这样剁下去，改来改去就7个字节。
有VirusTotal企业帐号的可以从VT下原包。

四哥原话在Bp破解上最大的贡献是演示了一种直接修改字节码的破解方式
```

**反编译jar For Linux**

```
-classpath <路径>            指定查找用户类文件和注释处理程序的位置

-d <目录>                    指定放置生成的类文件的位置

cd  burp-loader-keygen.jar.src

javac -classpath burp-loader-keygen.jar -d . enjoy/reversing/me/KeygenDialog.java
```

![](https://github.com/jas502n/BurpSuite_Pro_v1.7.37/blob/master/javac.jpg)

![](https://github.com/jas502n/BurpSuite_Pro_v1.7.37/raw/master/JD-GUI.jpg)

[参考jas502n](https://github.com/jas502n/BurpSuite_Pro_v1.7.37/blob/master/README.md)

> **其他**

**2020-04-28 17:23 scz -- 来自四哥博客**

- ```
  有人提供了Burp Pro 2020.4原包，要求最低Java 9，不再支持Java 8。实际测试
  Java 8确实不行，去官网看了一下说明，官方声明也是这个意思。出于好奇心，最后
  看了一次其注册机制，没啥变化，可剁。我主要使用Java 8，并非Burp用户，能在这
  半年来坚持更新破解，算是为大伙儿尽一点小小的心意。本来，如果它还支持Java 8，
  我就继续剁下去。不想为这事再装Java 9，确实累了，另一方面也对之失去兴趣，没
  有挑战性。据我所知，很多人延着我的思路在自己剁，也剁成功了。或许你们可以等
  待新的雷锋，冥冥中另一些路见不平的老中医已经在路上。
  
  正式决定不再从事Burp破解，微信订阅号后台也不再接受Burp原包。今天有ID为火锅
  爹、Mannix的两位在微信订阅号后台提供了2020.4版原包，感谢并抱歉，未能最后一
  次提供传说中的burp-loader-keygen-2020_4.jar。
  
  今天是一个有些伤感的日子，但不再留恋，再见。
  ```

**2020-03-24 15:01 scz -- 来自四哥博客**

- ```
  迭代太快，如无绝对必要，还是用老版吧。在我发了各次迭代对应的loader之后，
  终于有人开始自力更生提供同型loader，这是好事。不好的一点是，
  某些人只提供loader，不提供原包。老中医看不惯这些SB们，只好继续1024了。
  ```

**虽然四哥已经不再提供 keygen&loader，但四哥blog依旧坚持更新pro jar包下载地址**

> **某些错误**

```
JDK 9中不再支持用于指定引导类路径，-Xbootclasspath和-Xbootclasspath/p选项以及系统属性sun.boot.class.path

所以 Java9-Java14 要用 javaagent

JDK13虽然警告-noverify在之后的版本将被舍弃，但JDK14依旧可以用

Parrot / Kali：打开内置浏览器 --> Project options --> Misc --> Embedded Browser

Burp Suite 2020.11
    BUG：某些错误会导致Bp无法正常启动，遇到错误后再重新启动Bp无法加载现有项目

Burp Suite 2020.9
    BUG：WebSocket消息无法在消息编辑器中正确显示

Burp Suite 2020.8.1
    BUG：网络环境不佳，频繁无响应，需重启

Burp Suite 2020.8
    BUG：使用汉化可能存在闪退

Burp Suite 2020.4.1
    BUG：存在消息编辑器中文本重叠

Burp Suite 2020.4
    BUG：存在消息编辑器中文本重叠

Burp Suite 2020.2.1
    BUG：Burp Repeater中发送的每个请求的响应时间不可以正确显示【影响延时注入判定，没有响应时间】

Burp Suite 2020.1
    BUG：输入中文异常,中文乱码
```

> **Bp相关**

```
# Linux Bp激活信息保存位置
~/.java/.userPrefs/burp

# Linux Bp配置文件位置
~/.BurpSuite

# Windows Bp激活信息保存位置
注册表：HKEY_CURRENT_USER\Software\JavaSoft\Prefs\burp

# Windows Bp配置文件位置
C:\Users\%username%\AppData\Roaming\BurpSuite
```

*写在最后，以现有情况，这个git库可能不再更新，除非官方把网站下载方式再次调整，或者改变授权加密方式*
