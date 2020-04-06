---
layout: post
title: 红外线遥控
reward: false
date: 2020-04-05 23:17:24 +08:00
tags:	[hardware, ir]
---

# 红外线遥控学习及发送

---

## 红外发送
ir.transmit(frequency, codes)

红外发送接口

```
  var codes = new Uint32Array([32,32,12,34]);
  ir.transmit(38000, codes);
```

## 红外学习
 ir.learn(timeout, callback)
 
 红外学习接口
 
 ```
 ir.learn(1000, function(frequency, codes) {
 });
 ```

## 参考
* [NFC 接口](nfc)
* [蓝牙接口](bluetooth)

