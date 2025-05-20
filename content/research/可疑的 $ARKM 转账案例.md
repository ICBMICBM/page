+++
title = "可疑的 $ARKM 转账案例"
sort_by = "date"
date = 2025-05-20
+++
# 可疑的 $ARKM 转账案例

> 关于这篇文章：由 Jerry Peng 以英文编写，并由专职写手 Miko Ilas 润色；此中文翻译由Claude 3.7 sonnet 翻译，并经 Jerry Peng 审核。本文于编写时部分线索已被其它推特博主发现并发布，被抢先发布的线索已在文中提到抢先发布的博主和主体。文章在发布后引起相关代币30%的波动，Arkham CEO Miguel Morel 通过 0xScope CEO Phillip Torres 联系 Jerry Peng 并回答了相关问题，并且在此次交流后 Arkham 修改了代币锁定方式以使其更符合其代币经济学。本文最初发布于 [https://www.0xscope.com/blog-posts?slug=the-curious-case-of-suspicious-arkm-transfers](https://www.0xscope.com/blog-posts?slug=the-curious-case-of-suspicious-arkm-transfers)
> 

加密分析公司 Arkham 目前正受到加密社区的严密审查，此前加密侦探 @EmberCN 和竞争对手公司 Nansen 开始关注涉及 $ARKM 代币的近期交易。

4月3日，@EmberCN 注意到 2500 万 ARKM（约 6250 万美元）被解锁并从 Arkham 的生态系统基金和国库转出。其中，600 万*ARKM*（约 1500 万美元）被解锁并从 Arkham **的生态系统基金和国库转出。600 万 ARKM（ 1500 万美元）已被转入一家主要交易所。同时，根据 Nansen 在 4 月 5 日的推文线程，约 2520 万 $ARKM（价值约 5600 万美元）已转移到多个钱包，而这些钱包在 Arkham 的钱包追踪平台上未被标记。

为了揭示超出对 Arkham 最初指控的更大图景，0xScope 团队对近期 $ARKM 交易进行了更深入的调查和分析。

## **序言：$ARKM 上线 Coinbase + 看涨鲸鱼动向**

4月2日，ARKM 在 Coinbase 上市。当时， ARKM 被积极看涨，原因如下：

1. Coinbase 上市期间 $ARKM 的中心化交易所提币和充币显示提币所占比例更大，这对交易者来说可能是看涨信号。
2. 关键做市商增加了他们的 ARKM 持有量。例如，GSR 将其 $ARKM 持有量从 315 万增加到 1359 万枚。同时，GSR 用于处理中心化交易所充币的地址持有 32.1 万 $ARKM，高于之前的 7.9 万。
3. 另一家主要加密货币做市商 Wintermute 将其 $ARKM 持有量从 46.9 万增加到 202 万代币。
4. 4月1日（Coinbase上架 $ARKM 前一天），主要加密交易所的 $ARKM 交易未平仓合约增加了 14%。

然而，自Coinbase上市以来，Arkham 进行了一些至少可以说是令人费解的 $ARKM 转账。

![image.png](/images/arkm/image1.png)

## **可疑的 $ARKM 转账及其影响**

当 Arkham 首次发布 $ARKM 代币经济学时，它将其 10 亿总供应量 40.5% 的 $ARKM 分配给其投资者、核心贡献者以及顾问。这些代币按代币经济学应在上架交易所后锁定一年并在此后三年进行线性解锁。$ARKM 在 2023 年 7 月 18 日上架交易所，因此，第一次解锁应该在 2024 年 7 月进行。

然而，距离ARKM上市一周年还有约三个月时，Arkham 违反了其代币经济学条款。0xScope 团队概述了截至4月8日的ARKM代币实际流向：

![image.png](/images/arkm/image2.png)

根据我们的研究，只有 3.55 亿 $ARKM 在锁定合约中，远低于计划的 40.5% $ARKM*。*

以下是根据 0xScope 和其他调查人员独立进行的调查，对最近的 $ARKM 转账进行的细分：

1. 4月2日，Arkham 国库向地址 0x1411 发送了 2000 万 $ARKM（5200 万美元），该地址将 500 万$ARKM（5200万美元）转给了 0x0d25。这个地址随后向一家主要交易所的 Wintermute 存款地址存入了 100 万 $ARKM。0x0d25 仍持有 400 万 $ARKM，可能用于未来的抛售交易。更多详情，可以在 Scopescan 上查看此代币流向。

![image.png](/images/arkm/image3.png)

1. 同一天，Arkham 国库解锁了 20 万 $ARKM 并将其发送到地址 0x9eac。该地址尚未移动其持有的 $ARKM 资金。
2. 大约同时，Arkham 生态系统基金解锁并转移了 500 万 $ARKM，这些代币全部通过做市商 GSR 使用的多个地址进入了一家主流交易所，如此代币流向图所示。其中一个地址0xe5d6值得注意，GSR曾通过 Arbitrum 链使用它存入他们的 Xai（$XAI）代币。

![image.png](/images/arkm/image4.png)

1. 鉴于近期 $ARKM 的重大转账，我们建议关注持有大量 $ARKM 代币的地址，特别是那些 Arkham 似乎仍然控制的地址，以便提前应对这些鲸鱼地址可能触发的抛售。例如，2023 年 7 月 18 日，当 $ARKM 开始在主要交易所上市时，Arkham 将其 3000 万代币转移到 GnosisSafe 地址 0x0850。根据该 GnosisSafe 所有者进行的交易，我们得出结论，该 GnosisSafe 由 Arkham 拥有。截至今天，存储在该地址的3000万ARKM尚未转出。
2. 此外，在 [snapshot.org](http://snapshot.org) 上授权 Arkham 基金会将 2000 万 $ARKM 转移到国库池 1 的提案中，一个与 Arkham 相关的地址投了 9600 万票支持，确保总票数超过了 7000 万的法定人数要求。

![image.png](/images/arkm/image5.png)

## **更大的图景：代币经济学变化等**

现在我们对 $ARKM 交易有了更全面的了解，不仅仅是最近的交易，还深入研究了相关的历史交易，我们可以推断出 $ARKM 交易者应该注意的一些潜在阻力和后果。

0xScope 团队分析了 $ARKM 在最近代币转移后的潜在风险。

1. **破坏投资者信任**
    
    $ARKM 代币转移的第一个后果是有确凿证据表明 Arkham 没有遵循其代币首次亮相时安排的代币分配。以下是 Arkham 初始代币经济学与通过其最近交易揭示的实际分配的快速比较。通过其最近的行动，Arkham 最终破坏了大多数投资者的信任。该项目是否打算向其社区解释这些变化，或是继续过去几天似乎采取的不予置评政策，仍有待观察。
    
    ![image.png](/images/arkm/image6.png)
    
2. **对 $ARKM 交易的看跌影响**
    
    出于各种原因购买 $ARKM 的人现在必须面对项目的代币经济学计划不会被遵循的现实，这增加了代币在市场上被抛售的风险。除非 Arkham 主动纠正这种情况，否则这种关于代币分配的不确定性可能会对未来的ARKM交易造成阻力。
    
3. **对社区警惕性的呼吁**
    
    最终，Arkham 的最新发展对其建立的社区最为重要。Web3 对公司组织的新颖方法赋予了代币持有者对他们投资的项目发生的事情发言权。这就是 Scopescan 和 Scopechat 等 Web3 分析工具可以帮助加密投资者保持对其加密投资的警惕性的地方，通过调查不规则的动向并了解其投资组合中代币的最新鲸鱼动向等众多其他好处。