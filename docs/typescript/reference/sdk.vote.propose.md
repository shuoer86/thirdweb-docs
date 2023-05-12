---
slug: /reference/sdk.vote.propose
title: Vote.propose property
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

# Vote.propose property

Create Proposal

## Example

```javascript
// The description of the proposal you want to pass
const description = "This is a great proposal - vote for it!";
// You can (optionally) pass in contract calls that will get executed when the proposal is executed.
const executions = [
  {
    // The contract you want to make a call to
    toAddress: "0x...",
    // The amount of the native currency to send in this transaction
    nativeTokenValue: 0,
    // Transaction data that will be executed when the proposal is executed
    // This is an example transfer transaction with a token contract (which you would need to set up in code)
    transactionData: tokenContract.encoder.encode("transfer", [
      fromAddress,
      amount,
    ]),
  },
];

const proposal = await contract.propose(description, executions);
```

**Signature:**

```typescript
propose: {
        (description: string, executions?: ProposalExecutable[] | undefined): Promise<TransactionResultWithId<never>>;
        prepare: (description: string, executions?: ProposalExecutable[] | undefined) => Promise<Transaction<TransactionResultWithId<never>>>;
    };
```

## Remarks

Create a new proposal for token holders to vote on.