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

## 区块链安全基础

### `链平台攻击`

**SP01：网络层攻击**  
Todo

**SP02：共识层攻击**  
Todo

**SP03：RPC攻击**  
Todo

**SP04：其他攻击**  
Todo  

### `智能合约安全风险`

**SS01：重入攻击（Reentrancy）**：[Github](./vulnerability/smartContract/readme.md#重入攻击reentrancy)

**SS02：整型溢出漏洞（overflow）**：[Github](./vulnerability/smartContract/readme.md#整型溢出漏洞overflow)

**SS03：tx.origin漏洞**：[Github](./vulnerability/smartContract/readme.md#txorigin漏洞)

**SS04：拒绝服务攻击（DoS）**：[Github](./vulnerability/smartContract/readme.md#拒绝服务攻击dos)

**SS05：预言机操纵（Oracle Manipulation）**：[Github](./vulnerability/smartContract/readme.md#预言机操纵oracle-manipulation)

**SS06：闪电贷攻击（Flashloan）**：[Github](./vulnerability/smartContract/readme.md#闪电贷攻击)

## 智能合约安全模拟实战

### `Ethernaut靶场带练`

Todo

### `Capturetheether靶场带练`

Todo

### `Damn Vulnerable DeFi靶场带练`

Todo

## 智能合约安全事件分析

Todo

## 智能合约安全事件复现

### Getting Started

- Follow the [instructions](https://book.getfoundry.sh/getting-started/installation.html) to install [Foundry](https://github.com/foundry-rs/foundry).

- Clone and install dependencies:`git submodule update --init --recursive`

### List of Past DeFi Incidents

- [20240702 WMRP](./exploit/readme.md#20240702---wmrp)
- [20230513 SellToken](./exploit/readme.md#20230513---selltoken)
- [20230227 SwapX](./exploit/readme.md#20230227---swapx)
- [20230219 BABYDOLL](./exploit/readme.md#20230219---babydoll)
- [20230217 Dexible DeFi](./exploit/readme.md#20230217---dexible)  
- [20230216 Platypus](./exploit/readme.md#20230216---platypus)
- [20230130 BEVO](./exploit/readme.md#20230130---bevo)
- [20221020 HEALTH](./exploit/readme.md#20221020---health)  
- [20220808 EGDFinance](./exploit/readme.md#20220808---egdfinance)

## 公链平台漏洞分析

Todo

## 公链平台漏洞挖掘

Todo
