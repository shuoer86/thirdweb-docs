---
slug: /reference/sdk.marketplaceauction.cancellisting
title: MarketplaceAuction.cancelListing property
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

# MarketplaceAuction.cancelListing property

Cancel Auction Listing

## Example

```javascript
// The listing ID of the auction listing you want to cancel
const listingId = "0";

await contract.auction.cancelListing(listingId);
```

**Signature:**

```typescript
cancelListing: {
        (listingId: BigNumberish): Promise<Omit<{
            receipt: ethers.providers.TransactionReceipt;
            data: () => Promise<unknown>;
        }, "data">>;
        prepare: (listingId: BigNumberish) => Promise<Transaction<Omit<{
            receipt: ethers.providers.TransactionReceipt;
            data: () => Promise<unknown>;
        }, "data">>>;
    };
```

## Remarks

Cancel an auction listing on the marketplace