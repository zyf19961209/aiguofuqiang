# 爱国富强中机场常见线路解析

## 公有云服务商：

**AWS：**

* 亚马逊云计算服务（英语：Amazon Web Services，缩写为AWS），由亚马逊公司所创建的云计算平台，亚马逊AWS占全球云市场第一。
* AWS到联通和移动网速不佳。国际和本地带宽比较稳定。
* 新加坡和日本接了电信163，到电信延时有所改善。但是由于价格便宜，又很容易买到，所以到总体到国内质量还是比较差的。
* 但是由于价格便宜，又很容易买到，所以到总体到国内质量还是比较差的。不过这个价格下能做成这样真的已经非常良心（亏本）了。
* IP被墙重点关照很容易挂，但是浮动IP换起来也很方便。

  
  
**Azure:**

* Microsoft Azure是微软的公用云服务 \(Public Cloud Service\) 平台，规模仅次于亚马逊AWS。
* Azure 的带宽一般较大，部分实例的带宽可以达到 2Gbps。
* 本地和国际带宽很大很稳，去很多地方都会走自己的骨干网。
* 主要问题是目前黑卡用户比较多，到国内电信快被玩坏了，到联通目前还是打了鸡血一样的飞快，移动得看地方，大部分地区还不错。
* 还有个小毛病是播放YouTube的时候会默认走欧洲的CDN，所以油管测速不理想。

**阿里云**

* 阿里云，创立于2009年，是中国最大的云计算平台，服务范围覆盖全球200多个国家和地区。
* 阿里云香港和新加坡有接CN2、对电信用户来说应该是性价比最高的选择了。联通用户去香港不错，去新加坡绕上海出口。移动到新加坡还行，到香港虽然延迟低但是实测网速很难突破500Kb/S。
* 最大的问题是IP太容易被墙，当然也有很多方式可以降低被墙的概率，这里就不展开细说了。

**GCP:**

* Google云端平台（英语：Google Cloud Platform）是一项使用了Google核心基础架构、数据分析和机器学习技术的云计算服务。
* 到大陆的互联带宽较小，防御做得也不理想（我觉得这主要是大陆运营商的锅），经常到大陆断网或绕路，稳定性是最大问题。
* 国际带宽非常充裕，有自己的骨干网。
* 最近300美元不能重复撸了，感觉互联直连会有一定的回升。

### 地区常见服务器： <a id="&#x5730;&#x533A;&#x5E38;&#x89C1;&#x670D;&#x52A1;&#x5668;&#xFF1A;"></a>

### 香港： <a id="&#x9999;&#x6E2F;&#xFF1A;"></a>

**HKT：**

* 香港电讯有限公司，为电讯盈科（PCCW）旗下的一间子公司；
* HKT算是国内机场里最常见服务器了，一般都成为了机场的流量担当；
* 不过由于带宽价格相对低廉，已经被用于各种大流量业务，大陆方向已经被严重QoS，直连体验下滑。只有部分IP段完好，至于家宽商宽就不写了。

**PCCW：**

* 电讯盈科成立于2000年，为全港首屈一指的互连网服务供应商。
* 香港有一堆接了PCCW的商家，带宽单价比较高，所以目前很少有大带宽的PCCW线路了，基本上能买到的都是金针菇。唯一的大带宽的到国内走PCCW线路的可能只剩HKT了，被QOS之后也没那么值得购买了。

**HKBN:**

* 香港宽频是按用户数计算香港最大的光纤高速宽频住宅服务供应商；
* 不过HKBN大陆方向带宽总共只有5G，直连体验总体并不理想；

**香港阿里云：**

* 阿里云亚太轻量服务器，电信去程NTT绕日，只有回程是CN2；联通移动直连；
* 阿里云亚太ECS，电信双程CN2，联通移动直连。特别提示一下很多地方的移动到香港阿里云延迟漂亮但是速度很糟糕。
* 阿里云的海外服务器跑SS/SSR很容易被墙，现在的流量包都是绑定实例，换了浮动IP之后就不能用流量包了。

**Azure 香港：**

* AZ香港性价比之王，当然前提是黑卡不翻车的话。。
* 抗攻击非常到位良心

**LeaseWeb：**

* 国际和港内带宽大，稳定，到国内比较差劲，适合落地。
* 作为落地鸡用的话成本比较高，常见的销售香港LeaseWeb的商家如OneProvider流量给得比较少。
* 直接找官方购买独立服务器的话门槛较高，需要验证各种证件、地址证明，中国用户还会加收押金。

**SunnyVision：**

* 回国走PCCW，此机房自己本身QOS严重，上联带宽不足，价格挺贵的。
* 销售此机房VPS的商家不多，RFCHost，SV官方。总体上不太适合机场使用。

**Softlayer：**

* 国际和本地带宽不错，有自己的的全球骨干网。到国内绕得比较厉害。
* 官方售价高，二道贩子如HostUS（OpenVZ架构，不能bbr加速或锐速）价格虽然便宜，只是双向流量跟水一样不耐用，可以考虑用来落地。
* 注：虽然Softlayer本身的VPS抗攻击性能非常好，但是二道贩子那边摸一下就进黑洞至少24小时。

**HGC：**

* QOS之王的美誉不是吹出来的。不光是到大陆QOS严重，国际方向也有QOS。到国内网络质量比较一般，港内不错。
* 目前市面上卖的HGC小鸡价格都还可以（可能大家都不怎么喜欢用吧。。），可以考虑用来做落地。

**WTT：**

* 前两年刚有商家开始卖WTT商宽的时候到国内网络质量非常好，性价比无敌。
* 后来人多了就被玩坏了。人家运营商卖1G带宽的商宽不代表允许天天跑满大陆方向1G，所以网络被玩坏也是情理之中的事情。
* 最近大家都去撸HKT了，WTT这边估计人少的原因，到国内网络还不错。
* 价格不便宜，建议购买之前询问商家不满意是否可以退款。

**DMIT：**

* 在香港除阿里云之外为数不多的到大陆三网速度OK并相对稳定的IDC。
* 自己拉的CN2 transit，到大陆的互联质量是有一定保障的，不像HKT那样可能随时翻脸限速。

**Layerstack：**

* 问题较多，开个机都费劲，会出现重装之后无法开机等非常蛋疼的问题。
* 网络也比较迷，发起疯来连港内都可以限速的那种。
* 地雷警告：他家不接受退款要求，就算机器有问题连续一星期都用不了，也不接受退款。不是老司机的话不建议购买。  

香港永远是个是非之地。撸本地运营商翻车是大概率事件（WTT、HKT 血的教训）。建议购买自己直接拉大陆运营商的 transit 的商家。

### 日本： <a id="&#x65E5;&#x672C;&#xFF1A;"></a>

**纯 bbtec 类：**

* 此类典型的商家如阿里云日本，购买难度较高，价格较高。到大陆三网速度优秀，移动延迟稍微高一点。
* 价格中上，暂时还没被玩坏。考虑到目前日本可以买的选择太少了，被玩坏也只是时间问题。

**Azure 日本：**

* 主要走自己的骨干网到香港然后进入国内，网络质量可以参考Azure香港。
* 能撸黑卡并且不翻车的话性价比还是比较香的。

**Internap 全家桶类：**

* 此类一般是指去程bbtec，回程bbtec、iij、kddi随机。这个一般都不是特别稳，速度也比较一般。

**IIJ：**

* 到联通不错，移动一般，电信晚间延迟爆炸。不过价格便宜做个落地也不错。
* 性价比很高的IDCF最近开始不再对个人用户服务了，伤心。剩下值得买的大概也就GmoCloud了。

**AWS 日本：**

* AWS的日本区域拉了少量的163带宽，所以到电信还可以（带宽跑满照样会抽风）。不过这价格真的很良心了，不能再奢求更多了。

**KDDI：**

* 到大陆最近三网都飞快，因为基本上很少人能撸到。

**NTT：**

* 典型代表商家有Linode、Vultr这种大厂，也有官方云。总体国际互联很好，除了到大陆方向都很好。

**CN2：**

* 有一些卖日本CN2的商家，价格昂贵不太适合机场使用。

总体来说日本的本土商家比较排外。不要相信日本 VPS 所谓的 “无限流量”。比如 DataHotel 会在不做任何通知的情况下限速 100Kb/s。具体因为什么限速（或删号）他们的解释一般也是含糊其辞。总之性价比看起来太高的建议谨慎购买，一些日本商家比较排斥中国人搭梯子。国际大品牌在日本基本不存在这种问题，如 AWS、Linode、Azure、Vultr、阿里云之类的。

### 美国： <a id="&#x7F8E;&#x56FD;&#xFF1A;"></a>

**搬瓦工（GIA CN2）：**

* 可能是目前美西能直接无障碍买到的最清真的GIA CN2线路了。
* 价格不便宜，机场一般需要使用较大流量的套餐，成本还是比较高的。
* 胜在到国内总带宽较大，可以尽情的超售，比较稳定。
* 每隔一段时间可以免费更换被墙IP，否则收费换IP。
* 搬瓦工也算是GFW重点照顾单位，跑SS/SSR的话很容易被墙。建议充分考虑频繁被墙带来的额外成本与损失。

**RFCHost：**

* 在美西有C3和安畅两个机房可选（堪萨斯那个没测试过）。
* C3到国内主要走GT CN2，安畅到国内走GIA CN2。走GIA CN2会更稳更快。
* 老商家比较稳定，大部分时间处于缺货状态，佛系购买。

**Vultr：**

* 本地和国际带宽还不错，价格便宜，稳定性也不差。适合落地。配合流媒体解锁服务的话还是比较推荐的。
* 到国内互联质量比较差，IP也经常被GFW照顾，不建议直连。

**Linode：**

* Linode在美西只有Fremont机房，HE单线，国际和美国本土互联质量不如Vultr。
* 到国内的速度白天还行，晚上肯定是要爆炸的。不建议购买。

**DGCHost：**

* 应该算是最早的几家做洛杉矶GIA CN2的商家，超售率较高。
* 最大的问题可能是经常被攻击，稳定性不佳，不建议购买。

**GigsgigsCloud：**

* 到国内基本上是三网GIA CN2，超售厉害，碰到过多次小鸡宕机的情况，稳定性有待提高。

**Quadranet：**

* 至今不知道这货和Vultr这种相比有啥优势。

**NFOservers：**

* 到国内互联差，撸的中国人少，本地和国际带宽大，各种超大流量套餐其实性价比很不错。适合落地。

  
  
美国目前提供 GIA CN2 的商家其实有非常多，鱼龙混杂，小商家居多。  
这些主要只能看上游了。大部分上游集中在 C3、安畅、Quadranet。  
个人感觉安畅机房的会稳一点，可能是因为安畅机房的 CN2 资源是单独卖的。Quadranet 和 C3 的 GT CN2 好像都是大锅饭。

流媒体解锁推荐快车道家的 Fremont HE 单线不限流量服务器。价格相对合理，主要是不限流量，不需要担心 netflix 看多了会用完流量。其他一些商家如 RFCHost 的美西小鸡也是可以解锁流媒体的，但是流量给得较少。

_整理自：_[_https://www.duyaoss.com/index.php/archives/57/_](https://www.duyaoss.com/index.php/archives/57/)\_\_
