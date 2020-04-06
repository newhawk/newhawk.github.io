---
layout: post
title: NFC通信
reward: false
date: 2020-04-05 23:17:24 +08:00
tags:	[nfc]
---

# NFC卡读写

---

## nfc.card.read

# NFC卡模拟
---
## nfc.hce.startHCE
nfc.hce.startHCE(String[] aids)

```
  nfc.hce.startHCE(['12121']);
```

## nfc.hce.stopHCE

```
  nfc.hce.stopHCE()
```

## nfc.hce.onMessage

```
  nfc.hce.onMessage(function(data) {
    nfc.hce.sendMessage(reply);
  });
```

# NFC P2P通信
---

# NFC卡类型
## NfcA
NFC-A (ISO 14443-3A)

## NfcB
NFC-B (ISO 14443-3B)

Mifare标准，中国的二代身份证也是采用的该标准。

## NfcF
NFC-F (JIS 6319-4)

Felica标准，由SONY公司推出，是日本普遍采用的卡标准，如日本的公交卡等。


## NfcV
NFC-V (ISO 15693)

德州仪器的VicinityCard卡标准

## IsoDep
ISO-DEP (ISO 14443-4)

MIFARE DESFire

中国的公交卡、银行卡等都是采用这种标准。

## Ndef
NDEF

Android中文件分享，用的是该标准。

## NdefFormatable
NDEF formattable

## MifareClassic
MIFARE Classic

## MifareUltralight
MIFARE Ultralight


# 参考
* [红外遥控](ir)
* [蓝牙接口](bluetooth)

