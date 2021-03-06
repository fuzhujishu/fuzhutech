---
title: "如何使用有线方式连接用于转录文字的手机"
menutitle: "语音侧录线"
date: 2021-01-29T10:41:37-05:00
draft: false
---

当需要用手机为另一台设备提供字幕时，有线连接是目前最为可靠的办法。在将来，也许蓝牙连接也会成为另一种可用的方法。

使用时，在第一台手机上播放声音，用音频侧录线连接到第二台手机，并在第二台手机上打开 [语音转文字的 app]({{< ref "_index.md" >}}) 即可。也可以选择将音频流[一分二]({{< ref "#一分二" >}})，聆听与字幕转录同时进行。

如果使用这种音频线不能出字幕，可参考 [FAQ](#diy) 一节排查原因。

最后，我们简单讨论了一下如何用手机为电脑、电视、固定电话等其它设备提供字幕。

# 音频侧录线

用于这种用途的 3.5mm 音频接口侧录线有很多种名称。比如说 音书 就叫它“字幕音频线”。

这种线的原理非常简单。它有两头，一头接播放音频的设备（下文称音源侧），一头接用于提供字幕的手机（我们称字幕侧）。它将音源侧的耳机/扬声器的音频电平连接到字幕侧的麦克风接口上。

因此，虽然外观相似，但最常见的音频对录线是**不能**用于这种用途的，因为它们没有反接耳机线和麦克风线。

如果手头没有这种线，请见 [DIY](#DIY) 一节。

## 没有耳机接口怎么办

一般可以使用厂商或第三方提供的 USB/lightning 口转 3.5mm 音频接口转接线（或者叫 USB 声卡）。


{{% expand "小知识：USB 声卡" %}}
无论是 lightning 接口转 3.5mm，还是 microUSB 或者 USB Type-C 转 3.5mm，虽然常常被叫作“转接线”，但它们都是不折不扣的 USB 声卡。

但并不是所有的 USB 声卡都含有麦克风功能，没有麦克风功能的转接线只有 USB DAC，而没有 USB ADC。

显然，提供字幕的耳机这边必须购买支持麦克风的 USB 声卡。但输出声音的这一边买什么样的 USB 声卡都可以满足要求。
{{% /expand %}}

## 一分二

由于口语使用者往往还需要同时聆听输入端的声音，这种线一般还附带一分二功能，可以将分出的第二个接口用来接插扬声器或助听器/耳蜗的 streamer 之类设备。

如果买到的线没有带一分二功能，可以自己接一根 3.5mm 一分二音频线。

{{% expand "可以同时使用蓝牙耳机/助听器/耳蜗吗？" %}}
很遗憾的是，截止到 iOS 14，仍然蓝牙音频仍然不能与 USB 音频或内置 3.5mm 同时使用。也就是说，目前 iPhone **不可以**实现此功能。

Android 平台我们没有做全面的测试。已知部分华为手机无法同时使用有线和蓝牙。
{{% /expand %}}

## DIY

如果无法买到这种音频侧录线，也可以选择自己 DIY。

一种办法是买几根常见的线接起来。需要的线有以下几种

- 一根四格的 3.5mm 接口（3.5mm 耳麦接口）转成一个麦克风接口，一个耳机接口的一分二线。（不是普通的耳机线一分二线）
- 一根普通的公对公音频对录线
- 一根耳机一分二线，或者一分二插座。一头是公口，分出来两个耳机母口。

字幕侧手机插第一种线，音源侧手机插第三种线，然后使用第二种线将两边连接起来。音源侧手机还余一个耳机插口可以连耳机或者助听器 Streamer。

显然上面这种办法，原来一根特殊音频侧录线可以解决的问题，要变成很多根线。所以也可以自制音频侧录线。

首先买一根普通 3.5mm 公口对公口音频线，也叫音频对录线。插到字幕设备那一端的插头必须有 4 格而不是 3 格。如果只有 3 格的话，无法接到麦克风线上。然后在线中间拆开，将一路耳机线接到麦克风线上，重新封好即可。

为避免损伤麦克风，建议在麦克风线上串联一只 100 欧以上的电阻。虽然一般麦克风的输入阻抗都非常高，不接的话大概率也没有什么问题。

{{% expand "小知识：3.5mm 音频线标准之争" %}}
3.5mm 音频线有不同种类。传统单声道麦克风使用 2 格插头，一格是地线，一格是信号线。传统立体声耳机使用 3 格插头，一格是地线，每个声道各占一格。独立的立体声麦克风（不含耳机信号）使用相同的插头。

到手机上问题就来了，现在要在立体声耳机上加入麦克风信号，必然要再加一格。4 格 3.5mm 插头都是一样的，但到底哪一格是麦克风，哪一格是耳机，哪一格是地线，就有两种不同的标准。
中国的国家准备是 OMTP 标准，此标准是当年诺基亚所力推的。而世界其它市场上，绝大部分手机厂商已经转为支持苹果所支持的 CTIA 标准。

那么，岂不是侧录线也会有两种不同的接法？实际上，在国内销售的手机为了应对两种标准的乱局，一般都搭载了自适应芯片，无论按 CTIA 还是按 OMTP 接法，都可以自动识别。一般无需担心这个问题。对于部分国外购买的手机，有可能遇到这个问题。
{{% /expand %}}

# FAQ

接上线之后，无法出字幕怎么办？

请按如下顺序逐个排查原因。

1. 是否接反了？侧录线的两头必须按照说明插，不能将插字幕侧的插头插到音源侧。如果是这种情况，请掉换线的两头重新插。
2. 有些手机的麦克风输入电平阈值很低。如果是这种情况，只能把音源侧的手机音量尽可能调低，调到一格左右，就可以出字幕了。
2. 有一些手机和 USB 声卡会检测输出阻抗，拒绝输出声音给耳机以外的设备。这种情况请使用一分二线，并先插上耳机，确保耳机可以出声音，再插上字幕侧手机。顺序不可颠倒。如果阻抗合适的话，也可以用助听器/耳蜗的 streamer 代替耳机。
3. 有万用表的话，可以测试侧录线各端口是否导通，以排除接触不良、线材断裂等问题。
4. 对于比较古老的手机型号或者水货手机，可能会遇到上文所述的 OMTP 和 CTIA 的兼容问题。对此，可以选择 [DIY](#diy) 一根线，或者为字幕侧的手机买一个带有麦克风支持的 USB 声卡。
5. 非常不幸，但比较少见地，也可能是字幕侧对于麦克风的阻抗或者电压有要求而屏蔽了信号。这种情况也只能换一个 USB 声卡了。

# 为其它设备提供字幕

除了可以用一台手机为另一台手机提供字幕之外，也可以用它为其它设备提供字幕。

## 电脑

做法和手机完全相同，需要的线材也完全相同。

## 固定电话

除去前文所说的 3.5mm 音频侧录线外，还需要一个将电话音频信号转到 3.5mm 音频接口的转接盒。有的录音笔会自带这种转接盒，零买的话似乎不太容易找到。

如果想自己弄的话，可以买个 RJ11 水晶头（RJ11 就是电话线插头的名字），将电话听筒声音接出来分压后接到 3.5mm 音频线的麦克风线上。需要注意的是电话线的电压很高，务必要先分压后接上去，否则可能会烧坏手机声卡！这需要一点电路基础知识和焊接能力。如果读者不明白这段在说什么的话，请勿轻易尝试。

市面上有一种 RJ11 转 3.5mm 耳麦转接线。这种转接线不是很难找，因为很多话务员需要使用头戴耳麦而不是电话听筒来打电话。如果想用的话，同上，务必测量好转接线输出的电压然后再使用，以免烧坏手机声卡！打电话时，电压不应超过 2V，最好不超过 1V。

除专门设计的电话录音转接盒外，无论是 DIY 转接线还是用耳麦转接线，如果接到电话线上使用，则不要在振铃时接通手机。电话线的振铃电压比通话电压高很多。

下面一步是把转接盒插到电话上。如果是成品转接盒，按说明书操作。如果是 DIY 转接线，可以选择插到电话机的分机接口或听筒接口上。耳麦转接线一般是插到听筒接口上的。

无论哪种线，如果插到分机接口的话，需要关闭电话机的防盗线功能。

如果插到听筒接口上，则占用了电话机本身的听筒，无法接打电话。为解决这个问题，还需要再麻烦一下。要么选择外接一个麦克风，要么把听筒的线分出来仍用原来的听筒麦克风。耳机倒是好办，用音频侧录线一分二之后插耳机即可。总之没有直插电话线那么方便。
另一头使用前文所述的 3.5mm 音频侧录线连到手机上即可。但由于转接线的阻抗不一定满足字幕端手机的要求，可能有的手机能显示字幕，有的手机就不能显示字幕。

最后，将本文前面用于连接手机的音频侧录线接上，另一头接到字幂侧手机上。由于字幕侧手机可能会对麦克风输入的阻抗和电压有一定要求，这种办法不见得每台手机都能成功。

## 电视

对于有 3.5mm 音频输出接口的电视，做法和手机连接完全相同。如果电视没有 3.5mm 接口，但有 RCA 接口，可以很容易地买到 RCA 转 3.5mm 转接线。

有些电视没有模拟音频输出，只有数字音频输出。对于这种电视，就需要额外购买解码器了。无论是 HDMI、S/PDIF 还是数字同轴，都可以买到相应的音频解码器。

如果解码器集成了功率放大器的功能，则需要注意输出电压，先从最小音量开始试起。


