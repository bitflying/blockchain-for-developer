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

### 5. 九大比特币著名地址
感兴趣的人可以使用下面的地址进行测试。
1. 1A1zP1eP5QGefi2DMPTfTL5SLmv7DivfNa

    该地址属于比特币创始人中本聪  , 是比特币的创世地址, 共收到的比特币：65.44021956 BTC。我们在上面的例子中使用过该地址。

2. 1Ez69SnzzmePmZX3WpEzMKTrcBF2gpNQ55

    所有者为美国法警局，该地址内的比特币来自被查获的丝绸之路，后在第一次拍卖会中将币转移给中标人。此前，美国联邦政府一度被认为是比特币最大的持有者之一，仅次于中本聪。共收到的比特币：29,658.80913195 BTC

3. 1XPTgDRhN8RFnzniWCddobD9iKZatrvH4

    该地址属于比特币披萨之王 Laszlo，2010年5月22日，美国佛罗里达州程序员Laszlo Hanyecz，用 10000 BTC 买下了价值25美元的披萨（2个），这是现实世界中的第一笔比特币交易。共收到的比特币：81,432.09 BTC
    
4. 14rE7Jqy4a6P27qWCCsngkUfBxtevZhPHB

    该地址属于“法国女仆”，又名Carl M. Force，是美国联邦缉毒局的一名探员，在参与调查丝绸之路时，Force化名“法国女仆”利用职务之便勒索罗斯乌布利希，并将赃款汇入该地址内，但Force最终被抓住并遭到起诉。共收到的比特币：770 BTC

5. 1M8s2S5bgAzSSzVTeL7zruvMPLvzSkEAuv

    该地址发生了一笔历史上最大额的交易，一次性转移了500,000 BTC，创历史之最。共收到的比特币：500,000.00910387 BTC

6. 1GBwk2YJMDFqSVhTKygH8zUwV7jdoJhHHH

    该地址属于彭博新闻社记者马特·米勒（Matt Miller），在节目中，马特·米勒无意中将自己的比特币私钥暴露在摄像机前，一位细心的红迪网网友“milkywaymasta”截取到了这一幕，并扫描了二维码，将私钥中的比特币转移到自己的地址内，然后他将细节写到了Reddit上，并表示，如果米勒给他一个新的地址，他愿意归还这些比特币，后来他也的确这样做了。共收到的比特币：0.02930731 BTC。

    注：这是一个重要的事件，因为它显示出保护私钥的重要性，0.02910731 BTC先是转移到了milkywaymasta的地址1GkBw2o1ZeqsrbtVNbuBiqfoWd95Q2s6Ku，后来再次转移到米勒所控制的另一个地址内。

7. 1HB5XMLmzFVj8ALj6mfBsbifRoD4miY36v

    该地址所有者为维基解密，在遭到西方国家政府的经济封锁后，维基解密开始通过该地址接受比特币捐款。共收到的比特币：3,889.75533662 BTC

8. 1L2JsXHPMYuAa9ugvHGLwkdstCPUDemNCf

    Bitstamp遭窃的热钱包地址，黑客在2015年1月5日时陆续从该地址内盗取了大约19,000BTC 。共收到的比特币：19,943.19478503 BTC

9. 1EBHA1ckUWzNKN7BMfDwGTx6GKEbADUozX

    这个地址的所有者非常神秘，也非常富有，该地址是其9大关联地址中的一个，每个地址中包含了大约66000 BTC，表明该神秘老板拥有超过550,000 BTC 。共收到的比特币：66,233.73736962 BTC