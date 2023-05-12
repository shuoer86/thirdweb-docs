---
slug: /reference/sdk.token
title: Token class
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

# Token class

Create a standard crypto token or cryptocurrency.

## Example

```javascript
import { ThirdwebSDK } from "@thirdweb-dev/sdk";

const sdk = new ThirdwebSDK("{{chainName}}");
const contract = await sdk.getContract("{{contract_address}}", "token");
```

## Constructors

| Constructor                                                                                                      | Modifiers | Description                                               |
| ---------------------------------------------------------------------------------------------------------------- | --------- | --------------------------------------------------------- |
| [(constructor)(network, address, storage, options, abi, chainId, contractWrapper)](./sdk.token._constructor_.md) |           | Constructs a new instance of the <code>Token</code> class |

## Properties

| Property                                      | Modifiers           | Type                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           | Description                          |
| --------------------------------------------- | ------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------ |
| [abi](./sdk.token.abi.md)                     |                     | [Abi](./sdk.abi.md)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |                                      |
| [app](./sdk.token.app.md)                     |                     | [ContractAppURI](./sdk.contractappuri.md)&lt;TokenERC20&gt;                                                                                                                                                                                                                                                                                                                                                                                                                                                    |                                      |
| [burn](./sdk.token.burn.md)                   |                     | { (amount: string &#124; number): Promise&lt;Omit&lt;{ receipt: import("@ethersproject/abstract-provider").TransactionReceipt; data: () =&gt; Promise&lt;unknown&gt;; }, "data"&gt;&gt;; prepare: (amount: string &#124; number) =&gt; Promise&lt;[Transaction](./sdk.transaction.md)&lt;Omit&lt;{ receipt: import("@ethersproject/abstract-provider").TransactionReceipt; data: () =&gt; Promise&lt;unknown&gt;; }, "data"&gt;&gt;&gt;; }                                                                     | Burn Tokens                          |
| [burnFrom](./sdk.token.burnfrom.md)           |                     | { (holder: string, amount: string &#124; number): Promise&lt;Omit&lt;{ receipt: import("@ethersproject/abstract-provider").TransactionReceipt; data: () =&gt; Promise&lt;unknown&gt;; }, "data"&gt;&gt;; prepare: (holder: string, amount: string &#124; number) =&gt; Promise&lt;[Transaction](./sdk.transaction.md)&lt;Omit&lt;{ receipt: import("@ethersproject/abstract-provider").TransactionReceipt; data: () =&gt; Promise&lt;unknown&gt;; }, "data"&gt;&gt;&gt;; }                                     | Burn Tokens                          |
| [contractRoles](./sdk.token.contractroles.md) | <code>static</code> | readonly \["admin", "minter", "transfer"\]                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |                                      |
| [encoder](./sdk.token.encoder.md)             |                     | [ContractEncoder](./sdk.contractencoder.md)&lt;TokenERC20&gt;                                                                                                                                                                                                                                                                                                                                                                                                                                                  |                                      |
| [estimator](./sdk.token.estimator.md)         |                     | [GasCostEstimator](./sdk.gascostestimator.md)&lt;TokenERC20&gt;                                                                                                                                                                                                                                                                                                                                                                                                                                                |                                      |
| [events](./sdk.token.events.md)               |                     | [ContractEvents](./sdk.contractevents.md)&lt;TokenERC20&gt;                                                                                                                                                                                                                                                                                                                                                                                                                                                    |                                      |
| [history](./sdk.token.history.md)             |                     | [TokenERC20History](./sdk.tokenerc20history.md)                                                                                                                                                                                                                                                                                                                                                                                                                                                                |                                      |
| [metadata](./sdk.token.metadata.md)           |                     | [ContractMetadata](./sdk.contractmetadata.md)&lt;TokenERC20, typeof TokenErc20ContractSchema&gt;                                                                                                                                                                                                                                                                                                                                                                                                               |                                      |
| [mint](./sdk.token.mint.md)                   |                     | { (amount: string &#124; number): Promise&lt;Omit&lt;{ receipt: import("@ethersproject/abstract-provider").TransactionReceipt; data: () =&gt; Promise&lt;unknown&gt;; }, "data"&gt;&gt;; prepare: (amount: string &#124; number) =&gt; Promise&lt;[Transaction](./sdk.transaction.md)&lt;Omit&lt;{ receipt: import("@ethersproject/abstract-provider").TransactionReceipt; data: () =&gt; Promise&lt;unknown&gt;; }, "data"&gt;&gt;&gt;; }                                                                     | Mint Tokens for the connected wallet |
| [mintBatchTo](./sdk.token.mintbatchto.md)     |                     | { (args: { amount: string &#124; number; toAddress: string; }\[\]): Promise&lt;Omit&lt;{ receipt: import("@ethersproject/abstract-provider").TransactionReceipt; data: () =&gt; Promise&lt;unknown&gt;; }, "data"&gt;&gt;; prepare: (args: { amount: string &#124; number; toAddress: string; }\[\]) =&gt; Promise&lt;[Transaction](./sdk.transaction.md)&lt;Omit&lt;{ receipt: import("@ethersproject/abstract-provider").TransactionReceipt; data: () =&gt; Promise&lt;unknown&gt;; }, "data"&gt;&gt;&gt;; } | Mint Tokens To Many Wallets          |
| [mintTo](./sdk.token.mintto.md)               |                     | { (to: string, amount: string &#124; number): Promise&lt;Omit&lt;{ receipt: import("@ethersproject/abstract-provider").TransactionReceipt; data: () =&gt; Promise&lt;unknown&gt;; }, "data"&gt;&gt;; prepare: (to: string, amount: string &#124; number) =&gt; Promise&lt;[Transaction](./sdk.transaction.md)&lt;Omit&lt;{ receipt: import("@ethersproject/abstract-provider").TransactionReceipt; data: () =&gt; Promise&lt;unknown&gt;; }, "data"&gt;&gt;&gt;; }                                             | Mint Tokens                          |
| [platformFees](./sdk.token.platformfees.md)   |                     | [ContractPlatformFee](./sdk.contractplatformfee.md)&lt;TokenERC20&gt;                                                                                                                                                                                                                                                                                                                                                                                                                                          |                                      |
| [roles](./sdk.token.roles.md)                 |                     | [ContractRoles](./sdk.contractroles.md)&lt;TokenERC20, (typeof [Token.contractRoles](./sdk.token.contractroles.md))\[number\]&gt;                                                                                                                                                                                                                                                                                                                                                                              |                                      |
| [sales](./sdk.token.sales.md)                 |                     | [ContractPrimarySale](./sdk.contractprimarysale.md)&lt;TokenERC20&gt;                                                                                                                                                                                                                                                                                                                                                                                                                                          |                                      |
| [signature](./sdk.token.signature.md)         |                     | [Erc20SignatureMintable](./sdk.erc20signaturemintable.md)                                                                                                                                                                                                                                                                                                                                                                                                                                                      | Signature Minting                    |

## Methods

| Method                                                              | Modifiers | Description                                                                                                                                                                                                         |
| ------------------------------------------------------------------- | --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [getDelegation()](./sdk.token.getdelegation.md)                     |           | Get your voting delegatee address                                                                                                                                                                                   |
| [getDelegationOf(account)](./sdk.token.getdelegationof.md)          |           | Get a specific address voting delegatee address                                                                                                                                                                     |
| [getMintTransaction(to, amount)](./sdk.token.getminttransaction.md) |           | Construct a mint transaction without executing it. This is useful for estimating the gas cost of a mint transaction, overriding transaction options and having fine grained control over the transaction execution. |
| [getVoteBalance()](./sdk.token.getvotebalance.md)                   |           | Get your wallet voting power for the current checkpoints                                                                                                                                                            |
| [getVoteBalanceOf(account)](./sdk.token.getvotebalanceof.md)        |           |                                                                                                                                                                                                                     |
| [isTransferRestricted()](./sdk.token.istransferrestricted.md)       |           | Get whether users can transfer tokens from this contract                                                                                                                                                            |

**Signature:**

```typescript
export declare class Token extends StandardErc20<TokenERC20>
```

**Extends:** [StandardErc20](./sdk.standarderc20.md)&lt;TokenERC20&gt;