#!name= 🇹🇼Metflix
#!desc= netflix

[Script]
http-request ^https?://ios\.prod\.ftl\.netflix\.com/iosui/user/.+path=%5B%22videos%22%2C%\d+%22%2C%22summary%22%5D script-path=https://raw.githubusercontent.com/kwloufffl/NetflixTw/main/Twguoq, requires-body=true, timeout=10, tag=奈飞评分
http-response ^https?://ios\.prod\.ftl\.netflix\.com/iosui/user/.+path=%5B%22videos%22%2C%\d+%22%2C%22summary%22%5D requires-body=1,script-path=https://raw.githubusercontent.com/kwloufffl/NetflixTw/main/Twguoq, requires-body=true, timeout=10, tag=奈飞评分
http-response ^https?://ios\.prod\.ftl\.netflix\.com/iosui/warmer/.+type=show-ath script-path=https://raw.githubusercontent.com/kwloufffl/NetflixTw/main/Twguoq, requires-body=true, timeout=10, tag=奈飞评分

[MITM]
hostname = ios.prod.ftl.netflix.com
