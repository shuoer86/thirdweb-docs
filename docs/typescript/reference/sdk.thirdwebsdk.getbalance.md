---
slug: /reference/sdk.thirdwebsdk.getbalance
title: ThirdwebSDK.getBalance() method
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

# ThirdwebSDK.getBalance() method

Get the native balance of a given address (wallet or contract)

## Example

```javascript
const balance = await sdk.getBalance("0x...");
console.log(balance.displayValue);
```

**Signature:**

```typescript
getBalance(address: AddressOrEns): Promise<CurrencyValue>;
```

## Parameters

| Parameter | Type                                  | Description                          |
| --------- | ------------------------------------- | ------------------------------------ |
| address   | [AddressOrEns](./sdk.addressorens.md) | the address to check the balance for |

**Returns:**

Promise&lt;CurrencyValue&gt;