---
title: 配置项
sidebar: auto
---

## 必填

### 📌appID

* 对应 LeanCloud 创建的应用中的 AppID

### 📌appKEY

* 对应 LeanCloud 创建的应用中的 AppKEY

## 选填

### 📌severurl

* 如果你是国内版 LeanCloud 用户，此项必填
* 对应 LeanCloud 创建的应用中绑定的 API 域名。

### 📌slanguage

* 功能：语言设置
* 默认值：zh（中文）
* 可选项：en（英语），es（西班牙语）

对不同语言有需求的可以联系我

### 📌per

* 功能：每页显示说说的数量（也是每次加载说说的数量）
* 默认值：5
* 参数范围：>0

### 📌placeholder1

* 功能；在编辑说说的输入框中的占位符
* 默认值：无
* 参数类型：字符串

### 📌placeholder2

* 功能；自定义头像 url 的输入框的的占位符
* 默认值：无
* 参数类型：字符串

默认每条说说的头像按照 LeanCloud 用户中设置的头像显示，如果发布时在自定义头像 url 中填写自定义头像链接，会取代默认头像

### 📌lazy

* 功能：加载动画的开关
* 默认值：1（开启）
* 可选项：0（关闭），1（开启）

2.1 版本之后，不建议关闭加载动画

### 📌bgimg

* 功能：说说输入框背景图片
* 默认值：无
* 参数类型：图片的链接形式

### 📌color1 color2 color3

* 功能：说说的配色
* color1：说说背景颜色 1 & 按钮颜色 1
* color2：说说背景颜色 2 & 按钮颜色 2
* color3：说说字体颜色 1
* 默认值：demo 页中当前配色
* 参数类型：RGB 或十六进制

### 📌atemoji_array

* 功能：自定义表情包
* 默认值；无
* 参数类型：数组

JS 自带三套表情包（贴吧，bilibili小电视，QQ），分四页，最后一页为 custom，即用户自定义的表情包

### 📌gh_token

* 功能：自定义存储多媒体资源的 GitHub 账号 token（至少具有 write 权限，不建议添加其他权限）
* 默认值：为 Artitalk 的 GitHub 账号的 token
* 食用方法：在 User 表中设置的可发布说说的用户中添加名为 `gh_token` 的列，在里面填入 GitHub 的 token。

### 📌repo_pt_img

* 功能：自定义存储图片的仓库
* 默认值：/Artitalk/Artitalk-img/
* 格式；/GitHub用户名/仓库名/
  
### 📌repo_pt_mp3

* 功能：自定义存储音频的仓库
* 默认值：/Artitalk/Artitalk-mp3/
* 格式；/GitHub用户名/仓库名/
  
### 📌repo_pt_mp4

* 功能：自定义存储视频的仓库
* 默认值：/Artitalk/Artitalk-mp4/
* 格式；/GitHub用户名/仓库名/

### 📌cssurl

* 功能：自定义css接口
* 默认值：无
* 格式；链接形式，可根据仓库中的main.css魔改（注意：仓库中的main.css中的color1等换成你所需要的颜色即可）

## 配置项填写示例

```html
<script>
      var appID="ogP8qj3veMh0LFpFWMPOyF0X-MdYXbMMI";
      var appKEY="nHXLd3N3Jgh460t2iRQKWAtr";
      var placeholder1="Demo 页密码：123456";
      var per=2;
      var lazy=1;
      var slanguage="zh";
      var bgimg="https://cdn.jsdelivr.net/gh/drew233/cdn/20200409110727.webp";
      var atemoji_array={
            huaji: "https://cdn.jsdelivr.net/gh/moezx/cdn@3.1.9/img/Sakura/images/smilies/icon_huaji.gif",
            baiyan:"https://cdn.jsdelivr.net/gh/Artitalk/Artitalk-emoji/baiyan.png",
            bishi:"https://cdn.jsdelivr.net/gh/Artitalk/Artitalk-emoji/bishi.png",
            bizui:"https://cdn.jsdelivr.net/gh/Artitalk/Artitalk-emoji/bizui.png",
            chan:"https://cdn.jsdelivr.net/gh/Artitalk/Artitalk-emoji/chan.png"
      }
      var repo_pt_img="/Artitalk/Artitalk-img/";
      var repo_pt_mp3="/Artitalk/Artitalk-mp3/";
      var repo_pt_mp4="/Artitalk/Artitalk-mp4/";
</script>
```

注意：为避免不必要的 bug，不需要的配置项请不要进行定义

<ins class="adsbygoogle"
     style="display:block"
     data-ad-format="fluid"
     data-ad-layout-key="-fb+5w+4e-db+86"
     data-ad-client="ca-pub-9420537843748923"
     data-ad-slot="8405286900"></ins>
<script>
     (adsbygoogle = window.adsbygoogle || []).push({});
</script>
