---
slug: /sdk.gascostestimator.gaslimitof
title: GasCostEstimator.gasLimitOf() method
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

## GasCostEstimator.gasLimitOf() method

Estimates the gas limit of a transaction Pass in the same parameters as the contract's function.

## Example

```javascript
const gasLimitOfClaim = await nftDrop?.estimator.gasLimitOf("claim", [
  "0x...", // receiver
  1, // quantity
  "0x...", // currency
  1, // price per token
  [], // proofs
  1, // proof max quantity per transaction
]);
```

**Signature:**

```typescript
gasLimitOf(fn: keyof TContract["functions"] | (string & {}), args: Parameters<TContract["functions"][typeof fn]> | any[]): Promise<BigNumber>;
```

## Parameters

| Parameter | Type                                                                   | Description |
| --------- | ---------------------------------------------------------------------- | ----------- |
| fn        | keyof TContract\["functions"\] &#124; (string &amp; {})                |             |
| args      | Parameters&lt;TContract\["functions"\]\[typeof fn\]&gt; &#124; any\[\] |             |

**Returns:**

Promise&lt;BigNumber&gt;

the estimated gas limit of the transaction

## Remarks

Estimates the gas limit of a transaction