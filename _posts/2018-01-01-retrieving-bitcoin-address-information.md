---
layout: post
title:  "如何检索一个比特币地址的相关信息"
date:   2018-01-01
tags:  [比特币, 比特币地址, 区块链]
---
作为最早出现的加密币，它有着公共区块链的最重要的两个特性：私密性和公开透明性。
* 私密性：在比特币网络中，不包含任何用户的个人信息，比特币只与地址相关联，所以仅凭地址你是无法知道比特币的拥有者。
* 公开透明性：如果你知道某个人的比特币地址，你就能得到其在该地址下的多个重要信息，例如：
    * 当前有多少比特币
    * 曾经收到过多少个比特币
    * 曾经支付过多少个比特币 
    * 第一次使用该比特币地址的时间

下面我们指导大家，如何通过浏览器得到上述信息。
在测试过程中，我们使用的测试地址为1A1zP1eP5QGefi2DMPTfTL5SLmv7DivfNa，该地址属于比特币创始人中本聪, 是比特币的创世地址，地址内的比特币从未支付过。最初时，该地址内只有50币，后来一些爱好者不断地往该地址内转入少量BTC，以此表达对中本聪的敬意。

### 1. 获得比特币余额信息
* 打开浏览器，比如：谷歌的Chrome。
* 输入如下地址： https://blockchain.info/q/addressbalance/1A1zP1eP5QGefi2DMPTfTL5SLmv7DivfNa
* 得到结果如下： 6677245776， 结果是比特币的基本单位-satoshi， 而 1 BTC = 100,000,000 satoshi，所以该地址比特币余额是 66.77245776 个比特币。

### 2. 曾经收到的比特币数量
* 打开浏览器，输入如下地址： https://blockchain.info/q/getreceivedbyaddress/1A1zP1eP5QGefi2DMPTfTL5SLmv7DivfNa
* 得到结果如下： 6677245776，即 66.77245776 个比特币。

### 3. 曾经支付的比特币数量
* 打开浏览器，输入如下地址： https://blockchain.info/q/getsentbyaddress/1A1zP1eP5QGefi2DMPTfTL5SLmv7DivfNa
* 得到结果如下： 0，表示该地址从未支付过比特币给别人。

### 4. 第一次使用该比特币地址的时间
* 打开浏览器，输入如下地址： https://blockchain.info/q/addressfirstseen/1A1zP1eP5QGefi2DMPTfTL5SLmv7DivfNa
* 得到结果如下： 1231006505，表示系统时间，转换后为 Sun Jan  4 02:15:05 CST 2009， 即2009年1月4日
* 在Linux下，转换方法为：  date -d @"1231006505"
