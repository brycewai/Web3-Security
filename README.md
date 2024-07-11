# Web3 Security

**A Web3 Security Tutorial**

![img](./img/banner.png)  
有人说，Web3就像《三体》中的“黑暗森林”，那么该课程将带你进入“猎人”的门。

**Twitter:** [@brycewai](https://twitter.com/brycewai)  
**所有Github和教程开源在Github:** [https://github.com/BryceWai/Web3-Security](https://github.com/BryceWai/Web3-Security)

## 区块链基础

**F01：什么是区块链**：[Github](./basis/blockchain/readme.md)

**F02：区块链通用模型**：[Github](./basis/model/readme.md)

**F03：比特币模型详解**：[Github](./basis/btc/readme.md)

**F04：以太坊模型详解**：[Github](./basis/ethereum/readme.md)

**F05：常用工具和资料汇总**：Github

## Solidity

### `Solidity 入门`

本着不重复造轮子的理念，在此向大家推荐[WTF Academy - Solidity入门](https://wtf.academy/solidity-start)

### `Solidity 进阶`

本着不重复造轮子的理念，在此向大家推荐[WTF Academy - Solidity 进阶](https://wtf.academy/solidity-advanced)

## 常见协议和提案

### `Token`

[ERC 20](https://ethereum.org/en/developers/docs/standards/tokens/erc-20/)

[ERC 721](https://ethereum.org/en/developers/docs/standards/tokens/erc-721/)

[ERC 777](https://ethereum.org/en/developers/docs/standards/tokens/erc-777/)

[ERC 1155](https://ethereum.org/en/developers/docs/standards/tokens/erc-1155/)

### `安全相关提案`

[ERC 155](https://eips.ethereum.org/EIPS/eip-155)

[ERC 191](https://eips.ethereum.org/EIPS/eip-191)

[ERC 712](https://eips.ethereum.org/EIPS/eip-712)

## 区块链安全与审计

### `链平台安全审计`

| 序号 | 安全类型 | 安全子项 | 描述 | 危害等级 | 危害 |
| :-: | :-: | :-: | :-- | :-: | :-- |
| 1 | 编程语言 | 整数溢出 | 检查整数上溢和整数下溢 | High | 整数溢出可能会导致非常严重的逻辑错误、安全机制绕过等 |
| 2 |  | 死循环 | 检查程序的循环判断条件是否合理 | Medium | 死循环会导致程序卡死，最终被系统杀死 |
| 3 |  | 无限递归调用 | 检查程序递归调用的退出条件是否合理 | Medium | 导致节点崩溃 |
| 4 |  | 竞争条件 | 检查在并发状态下，对共享资源的访问操作 | Medium | 依具体情况分析 |
| 5 |  | 异常崩溃 | 检查能让程序主动退出的异常抛出代码 | Medium | 导致节点崩溃 |
| 6 |  | 除0漏洞 | 检查是否有除以0的情况 | Medium | 导致节点崩溃 |
| 7 |  | 类型转换 | 检查类型转换是否正确，转换过程中是否丢失重要信息 | Low | 依具体情况分析 |
| 8 |  | 数组越界 | 检查是否访问超出数组界限的元素 | Medium | 导致节点崩溃 |
| 9 |  | 反序列化漏洞 | 检查反序列化过程中有没有问题 | Medium | 依具体情况分析 |
| 10 |  | 不同编程语言独有的漏洞 | 检查和编程语言相关的漏洞 |  |  |
| 11 | 代码质量和可审计性 | 代码是否被比较好的组织 | 检查源码结构和模块化程度 | Info | 影响安全审计和代码维护 |
| 12 |  | 文档是否齐全 | 检查官网文档、源码内的文档、代码里的注释等是否齐全 | Info | 影响安全审计 |
| 13 |  | 测试代码覆盖率是否足够 | 检查测试代码是否覆盖了所有重要功能 | Info | 更容易出现安全问题 |
| 14 | RPC接口 | 功能实现安全 | 检查各RPC接口实现是否存在安全隐患，是否与RPC接口功能设计相符 | Medium | 造成节点崩溃、节点钱包被盗 |
| 15 |  | 敏感RPC接口权限设置是否合理 | 检查敏感RPC接口的访问权限设置 | Low | 敏感信息泄漏，任意签发交易，影响资产安全等 |
| 16 |  | 加密传输机制 | 检查是否用加密传输协议，比如TLS等 | Low | 造成敏感信息泄露 |
| 17 |  | 请求数据格式解析 | 检查对请求数据的格式解析过程 | Medium | 造成节点奔溃 |
| 18 |  | 钱包解锁攻击（黑色情人节攻击） | 节点解锁其钱包的时候，被RPC请求窃取资金 | High | 节点资金损失 |
| 19 |  | 传统Web安全 | 检查是否存在以下漏洞：跨站点脚本 （XSS） / 模板注入 / 第三方组件漏洞 / HTTP 参数污染 / SQL 注入 / XXE 实体注入 / 反序列化漏洞 / SSRF 漏洞 / 代码注入 / 本地文件包含 / 远程文件包含 / 命令执行注入等传统漏洞 | Medium | 依具体情况分析 |
| 20 | p2p网络 | 网络节点身份认证和识别机制 | 检查是否存在节点身份识别机制，节点身份识别机制能否被绕过 | Low | 依具体情况分析 |
| 21 |  | 加密传输机制 | 检查是否用加密传输协议，比如TLS等 | Low | 造成敏感信息泄露 |
| 22 |  | 路由表污染 | 检查路由表是否能够被随意插入或覆盖数据 | Low | 降低日食攻击等的难度 |
| 23 |  | 节点发现算法 | 检查节点发现算法是否均衡且不可预测，比如距离算法不平衡等问题 | Low | 依具体情况分析 |
| 24 |  | 连接数占用审计 | 检查p2p网络连接节点数的限制和管理是否合理 | Low | 可导致节点拒绝服务 |
| 25 |  | 日蚀攻击 | 评估日食攻击的成本与危害，必要时提供量化分析 | High | 隔离正常节点，资产双花，严重者可导致链回滚、链分叉等问题 |
| 26 |  | 女巫攻击 | 评估投票共识机制，分析投票资格检查策略 | Low | 虚假节点可以像真正的节点一样，对网络产生不成比例的巨大影响。这可能会导致其他几种攻击，如 DoS、DDoS 等 |
| 27 |  | 窃听攻击（Eavesdropping Attack） | 检查通信协议是否泄露隐私 | Low | 攻击者可以使用此私人信息危害网络中的节点、中断路由或降低应用程序性能 |
| 28 |  | 异形攻击 | 评估节点是否能识别同类链节点 | Low | 导致节点离线、通信延迟、通信效率降低 |
| 29 |  | 时间劫持 | 检查节点的网络时间计算机制 | High | 依具体情况分析 |
| 30 | DoS攻击审计 | 内存耗尽攻击 | 检查大内存消耗的地方，特别是解压缩的代码 | Medium | 导致节点崩溃 |
| 31 |  | 硬盘耗尽攻击 | 检查大文件存储的地方，特别是将数据解压缩到本地的代码 | Medium | 导致节点硬盘被无用数据占满 |
| 32 |  | socket压力攻击 | 检查链接数量的限制策略 | Medium | 导致节点拒接合法请求 |
| 33 |  | 内核句柄耗尽攻击 | 检查内核句柄创建的限制，比如文件句柄等 | Medium | 导致节点拒绝合法请求 |
| 34 |  | 数据包大小是否有合理限制 | 检查请求数据包的大小限制 | Low | 可能导致节点崩溃 |
| 35 |  | 持续性的内存泄露 | 检查内存泄露的地方 | Low | 可能导致节点崩溃 |
| 36 | 密码学 | 哈希算法安全性 | 检查哈希算法的抗碰撞性 | Medium | 依具体情况分析 |
| 37 |  | 数字签名算法安全性 | 检查签名算法安全性，算法实现的安全性 | Medium | 依具体情况分析 |
| 38 |  | 加密算法安全性 | 检查加密算法安全性，算法实现的安全性 | Medium | 依具体情况分析 |
| 39 |  | 随机数生成器安全性 | 检查关键随机数生成算法是否合理 | Medium | 依具体情况分析 |
| 40 |  | 侧信道攻击审计 | 检查算法中与时间消耗相关的逻辑，防止侧信道泄露密钥信息 | Medium | 密钥信息被猜到 |
| 41 | 共识机制 | BFT实现安全 | 评估BFT算法的实现安全性 | High | 导致投票机制绕过 |
| 42 |  | 分叉选择规则 | 检查分叉选择规则以确保安全性 | High | 依具体情况分析 |
| 43 |  | 网络分区 | 评估网络分区情况下的行为和影响 | Medium | 导致中心化安全性降低 |
| 44 |  | 中心化程度检测 | 鉴别系统设计中是否存在过度中心化设计 | Medium | 依具体情况分析 |
| 45 |  | 激励机制审计 | 评估激励机制对安全性的影响 | Medium | 依具体情况分析 |
| 46 |  | 双花攻击 | 检查共识是否可以防御双花攻击 | High | 依具体情况分析 |
| 47 |  | MEV攻击审计 | 检查区块打包节点的MEV对链公平的影响 | Low | 依具体情况分析 |
| 48 | 区块 | 区块同步过程审计 | 检查同步过程中的安全问题 | Medium | 依具体情况分析 |
| 49 |  | 区块格式解析过程审计 | 检查格式解析过程中的安全问题，比如解析错误导致奔溃 | Medium | 造成节点崩溃 |
| 50 |  | 区块生成过程审计 | 检查区块生成过程中的安全问题，包括Merkle tree root构建方式是否合理 | High | 依具体情况分析 |
| 51 |  | 区块校验过程审计 | 检查区块签名内容项及验证逻辑是否充分 | High | 导致区块伪造 |
| 52 |  | 区块确认逻辑审计 | 检查区块确认算法及实现是否合理 | High | 链回滚、链分叉 |
| 53 |  | 区块哈希碰撞 | 检查区块哈希碰撞的构造方式，及碰撞时的处理是否合理 | Medium | 依具体情况分析 |
| 54 |  | 区块处理资源限制 | 检查孤儿区块池、验证计算、硬盘寻址等资源限制是否合理 | Medium | 造成节点大量资源消耗 |
| 55 | 交易 | 交易同步过程审计 | 检查同步过程中的安全问题 | Medium | 依具体情况分析 |
| 56 |  | 交易哈希碰撞 | 检查交易哈希碰撞的构造方式，及碰撞时的处理 | High | 依具体情况分析 |
| 57 |  | 交易格式解析 | 检查格式解析过程中的安全问题，比如解析错误导致奔溃 | Medium | 造成节点崩溃 |
| 58 |  | 交易合法性校验 | 检查各类型交易签名内容项及验证逻辑是否充分 | High | 造成交易伪造 |
| 59 |  | 交易处理资源限制 | 检查交易池、验证计算、硬盘寻址等资源限制是否合理 | Medium | 造成节点大量资源消耗 |
| 60 |  | 交易延展性攻击 | 交易是否可以改变内部字段(比如ScriptSig)从而改变交易hash而不影响交易的有效性 | Medium | 依具体情况分析 |
| 61 |  | 交易重放攻击审计 | 检查系统对交易重放的检测 | High | 造成双花等 |
| 62 | 合约虚拟机 | 合约字节码校验 | 检查虚拟机校验合约的过程的安全问题，比如整数溢出、死循环等 | High | 造成节点崩溃 |
| 63 |  | 合约字节码执行 | 检查虚拟机执行字节码的过程的安全问题，比如整数溢出、死循环等 | High | 造成节点崩溃 |
| 64 |  | gas模型 | 检查交易处理/合约执行的各原子操作对应的手续费是否与资源消耗成正比 | Info | 影响系统公平 |
| 65 | 日志系统 | 日志记录的完整性 | 检查关键信息是否被日志记录 | Info | 导致无法跟踪节点关键信息 |
| 66 |  | 日志记录的安全性 | 检查处理日志的过程中，是否因处理不当造成安全问题，比如整数溢出等 | Medium | 依具体情况分析 |
| 67 |  | 日志包含隐私信息 | 检查日志是否包含密钥等隐私信息 | Medium | 敏感信息泄露 |
| 68 |  | 日志存储不占用过多内存和硬盘 | 检查日志是否记录过多内容，导致节点资源消耗 | Medium | 可能导致节点拒绝服务 |
| 69 | 供应链（三方库使用安全） | 节点代码供应链安全 | 检查所有第三方库、组件及公链框架对应版本的已知问题 | Info | 依具体情况分析 |

### `智能合约安全漏洞`

**SS01：重入攻击（Reentrancy）**：[Github](./vulnerability/smartContract/readme.md#重入攻击reentrancy)

**SS02：整型溢出漏洞（overflow）**：[Github](./vulnerability/smartContract/readme.md#整型溢出漏洞overflow)

**SS03：tx.origin漏洞**：[Github](./vulnerability/smartContract/readme.md#txorigin漏洞)

**SS04：拒绝服务攻击（DoS）**：[Github](./vulnerability/smartContract/readme.md#拒绝服务攻击dos)

**SS05：预言机操纵（Oracle Manipulation）**：[Github](./vulnerability/smartContract/readme.md#预言机操纵oracle-manipulation)

**SS06：闪电贷攻击（Flashloan）**：[Github](./vulnerability/smartContract/readme.md#闪电贷攻击)

## 智能合约安全事件分析

Todo

## 智能合约攻击Exp

### 安装 Foundry

- Follow the [instructions](https://book.getfoundry.sh/getting-started/installation.html) to install [Foundry](https://github.com/foundry-rs/foundry).

- Clone and install dependencies:`git submodule update --init --recursive`

### 攻击事件 Exp

- [20240702 WMRP](./exploit/readme.md#20240702---wmrp)
- [20230513 SellToken](./exploit/readme.md#20230513---selltoken)
- [20230227 SwapX](./exploit/readme.md#20230227---swapx)
- [20230219 BABYDOLL](./exploit/readme.md#20230219---babydoll)
- [20230217 Dexible DeFi](./exploit/readme.md#20230217---dexible)  
- [20230216 Platypus](./exploit/readme.md#20230216---platypus)
- [20230130 BEVO](./exploit/readme.md#20230130---bevo)
- [20221020 HEALTH](./exploit/readme.md#20221020---health)  
- [20220808 EGDFinance](./exploit/readme.md#20220808---egdfinance)

## 公链平台漏洞挖掘

[Beosin发现Move VM严重级别漏洞：可导致 Sui、Aptos 等公链全网崩溃，甚至可能硬分叉](https://mp.weixin.qq.com/s/n3EPv8lMHaNXoYICz9M6lg)

[Beosin硬核安全研究 | 内存炸弹漏洞导致Sui节点崩溃？](https://mp.weixin.qq.com/s/Gzh2c6hWpEWx47yXlZaXoQ)

## ZK 零知识证明安全

[ERC | ERC-7520草案：zk-SNARK公共输入溢出攻击防护](https://mp.weixin.qq.com/s/Iq3avRV7z05-ku4XMZZGSg)

[CVE | Beosin 提交Circom 验证库漏洞CVE-2023-33252，并附修复方案，zk项目方需警惕！](https://mp.weixin.qq.com/s/X09QL3QPs-7SatqgQbImiA)

[ZKP | 电路审计：冗余约束真的冗余吗？](https://mp.weixin.qq.com/s/fCooq4z2C81b5gQL2wQT4g)

[ZKP | 深度剖析零知识证明zk-SNARK漏洞：为什么零知识证明系统并非万无一失？](https://mp.weixin.qq.com/s/uBydpXnHLSROQokHr01S3g)

[ZKP | 深入探究 Tornado.Cash，揭示zkp项目的延展性攻击](https://mp.weixin.qq.com/s/-f5sF4U66iIZVVwig8JOgA)

[ZKP | 3种针对ZK基础算法Groth16的攻击手法分享](https://mp.weixin.qq.com/s/CIuhR8bHHjzR1garBBfq1g)
