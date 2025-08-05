---
title: misc
---

未特别说明情况下请求域名均为 https://chat-go.jwzhd.com
没写请求/响应项目表示不需要相关参数.  

## 获取个人表情收藏

GET /v1/misc/configure-distribution

请求头:  

|名称|必须|备注|
|-----|-----|-----|
|token|是|无|

响应体:  
```JSONC
{
  "code": 1, // 请求状态码，1为正常
  "data": {
    "audioUrl": "https://chat-audio1.jwznb.com/", // 音频路由
    "fileUrl": "https://chat-file.jwznb.com/", // 文件路由
    "imageUrl": "https://chat-img.jwznb.com/", // 图片路由
    "serverUrl": "http://chat.jwznb.com:8888/", // 未知
    "shareUrl": "https://yhfx.jwznb.com/", // 分享链接路由
    "videoUrl": "https://chat-video1.jwznb.com/", // 视频路由
    "websocketUrl": "wss://chat-ws-go.jwzhd.com/ws" // ws路由
  },
  "msg": "success" // 返回消息
}
```
