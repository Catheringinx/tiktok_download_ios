一、准备事项

1、制作tiktok.ipa

2、上传tiktok.plist.xml到宝塔

3、上传tiktok_onekey_install.html到宝塔

二、安装及后续

1、IOS打开：https://freshare.ga/tiktok_onekey_install.html （可能会更新）

2、点击tiktok一键在线安装

3、appstore安装任意一个免费应用

4、打开tiktok

5、卸载免费应用

6、打开小火箭 添加写入以下配置
[URL Rewrite]
(?<=_region=)CN(?=&) JP 307
(?<=&mcc_mnc=)4 2 307
^(https?:\/\/(tnc|dm)[\w-]+.\w+.com\/.+)(\?)(.+) $1$3 302
(^https?:\/\/*.\w{4}okv.com\/.+&.+)(\d{2}.3.\d)(.+) $118.0$3 302

[MITM]
hostname = .tiktokv.com,.byteoversea.com,*.tik-tokapi.com

7、安装证书

8、信任证书

9、重新打开并登录tiktok

8、代码可改地区（配置文本修改区号）

美国 - US
英国 - UK
韩国 - KR
日本 - JP
台湾 - TW
新加坡 - SG
