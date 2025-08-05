---
title: product-recommend/云湖金币活动商品
---

未特别说明情况下请求域名均为 https://chat-go.jwzhd.com
没写请求/响应项目表示不需要相关参数.  

## 获取

POST /v1/coin/shop/product-recommend

请求头:  

|名称|必须|备注|
|-----|-----|-----|
|token|是|无|

请求体:  
```JSONC
{
  "size": 100, // 字号
  "page": 1 // 商品页数
}
```

响应体:  
```JSONC
{
  "code": 1, // 请求状态码，1为正常
  "data": {
    "list": [
      {
        "id": 1, // 商品id
        "type": 1, // 
        "cycle": 7, //会员持续时间（持续7天
        "info": "7", 
        "name": "【云湖】会员7天", // 商品名
        "imageUrls": "[\"https://chat-img.jwznb.com/999955a351c67b761ed078dc40d28ede.png\"]", //商品图片url
        "price": 100, // 价格（单位为金币）
        "priceVip": 90, // vip专项价格
        "stock": 49, // 商品库存
        "sale": 0, // 已经出售了0件
        "description": "云湖会员7天，享受所有会员服务\r\n\r\n### **商品不定期补充库存，请留意全员群及官方消息**\r\n##### 注意事项\r\n1. 该商品每7天可兑换一次\r\n2. 兑换后直接开通或续费会员，无额外操作\r\n3. 虚拟商品，兑换后不支持退换\r\n4. 如有疑问联系官方客服", // 商品描述
        "delTime": 0, // 商品下架时间
        "createTime": 0, // 商品上架时间
        "lastUpdate": 0 // 商品更新时间
      }
    ],
    "total": 1 // 商品总数
  },
  "msg": "success" // 返回消息
}
```
