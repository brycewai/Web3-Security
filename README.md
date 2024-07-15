# Web3 Security

**A Web3 Security Tutorial**

![img](./img/banner.png)  

**Twitter:** [@brycewai](https://twitter.com/brycewai)  
**所有Github和教程开源在Github:** [https://github.com/BryceWai/Web3-Security](https://github.com/BryceWai/Web3-Security)

## 区块链基础

**F01: [什么是区块链](./basis/blockchain/readme.md)**

**F02: [区块链通用模型](./basis/model/readme.md)**

**F03: [比特币模型详解](./basis/btc/readme.md)**

**F04: [以太坊模型详解](./basis/ethereum/readme.md)**

**F05: [常用工具和资料汇总](https://brycewai.github.io/2022/08/07/%E5%8C%BA%E5%9D%97%E9%93%BE%E5%B8%B8%E7%94%A8%E5%B7%A5%E5%85%B7%E5%92%8C%E8%B5%84%E6%96%99/)**

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

**CS01: [公链安全审计项](./vulnerability/chain/readme.md#公链安全审计项)**

### `智能合约安全漏洞`

**SS01: [重入攻击（Reentrancy）](./vulnerability/smartContract/readme.md#重入攻击reentrancy)**

**SS02: [整型溢出漏洞（overflow）](./vulnerability/smartContract/readme.md#整型溢出漏洞overflow)**

**SS03: [tx.origin漏洞](./vulnerability/smartContract/readme.md#txorigin漏洞)**

**SS04: [拒绝服务攻击（DoS）](./vulnerability/smartContract/readme.md#拒绝服务攻击dos)**

**SS05: [预言机操纵（Oracle Manipulation）](./vulnerability/smartContract/readme.md#预言机操纵oracle-manipulation)**

**SS06: [闪电贷攻击（Flashloan）](./vulnerability/smartContract/readme.md#闪电贷攻击)**

## 智能合约安全事件分析

Todo

## 智能合约攻击Exp

### 安装 Foundry

- 跟随指引[instructions](https://book.getfoundry.sh/getting-started/installation.html) 安装[Foundry](https://github.com/foundry-rs/foundry).

- 复制下面的命令，安装子模块:  
`git submodule update --init --recursive`

### 攻击事件 Exp

[202407 LW](./exploit/readme.md#202407---lw)

[202407 WMRP](./exploit/readme.md#202407---wmrp)

[202305 SellToken](./exploit/readme.md#202305---selltoken)

[202302 SwapX](./exploit/readme.md#202302---swapx)

[202302 BABYDOLL](./exploit/readme.md#202302---babydoll)

[202302 Dexible DeFi](./exploit/readme.md#202302---dexible)

[202302 Platypus](./exploit/readme.md#202302---platypus)

[202301 BEVO](./exploit/readme.md#202301---bevo)

[202210 HEALTH](./exploit/readme.md#202210---health)

[202208 EGDFinance](./exploit/readme.md#202208---egdfinance)

## 公链平台漏洞挖掘

[MOVEVM | Beosin发现Move VM严重级别漏洞：可导致 Sui、Aptos 等公链全网崩溃，甚至可能硬分叉](https://mp.weixin.qq.com/s/n3EPv8lMHaNXoYICz9M6lg)

[SUI | 内存炸弹漏洞导致Sui节点崩溃](https://mp.weixin.qq.com/s/Gzh2c6hWpEWx47yXlZaXoQ)

## ZK 零知识证明安全

[ERC | ERC-7520草案：zk-SNARK公共输入溢出攻击防护](https://mp.weixin.qq.com/s/Iq3avRV7z05-ku4XMZZGSg)

[CVE | Beosin 提交Circom 验证库漏洞CVE-2023-33252，并附修复方案，zk项目方需警惕！](https://mp.weixin.qq.com/s/X09QL3QPs-7SatqgQbImiA)

[ZKP | 电路审计：冗余约束真的冗余吗？](https://mp.weixin.qq.com/s/fCooq4z2C81b5gQL2wQT4g)

[ZKP | 深度剖析零知识证明zk-SNARK漏洞：为什么零知识证明系统并非万无一失？](https://mp.weixin.qq.com/s/uBydpXnHLSROQokHr01S3g)

[ZKP | 深入探究 Tornado.Cash，揭示zkp项目的延展性攻击](https://mp.weixin.qq.com/s/-f5sF4U66iIZVVwig8JOgA)

[ZKP | 3种针对ZK基础算法Groth16的攻击手法分享](https://mp.weixin.qq.com/s/CIuhR8bHHjzR1garBBfq1g)
