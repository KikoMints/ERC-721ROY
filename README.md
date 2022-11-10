# ERC-721ROY

The best builders in the metaverse support creator royalties. The wisest ones will reward marketplaces that also support royalties. This symbiotic relationship is crucial for the health of the metaverse.

Introducing ERC-721ROY, a new standard that makes it all possible.

## Basic Functions

Add functions to ERC-721 that allow…
* a token owner to add their token(s) for sale
* a collector to buy tokens on sale
* a contract owner to collect royalties on sales

## Benefits

* Anyone can easily purchase your NFT directly on contract (no third party needed)
* List your NFT *once* for all marketplaces to query (no more listing on multiple marketplaces)
* `approvalForAll` is no longer needed, reducing scam effectiveness (scammers are trash 🤮)
* Bulk listing/buying means gas savings

## Additional Functions

We should add additional features that allow…
* a collector to bid on an NFT/collection by staking their eth
* a token owner to accept a bid
* a contract owner to reward marketplaces a % of collected royalties

And of course, a way to remove all your listings/bids

## Incentivizing Marketplace Development

NFT creators need to incentivize marketplaces to list their collection. This is simple: creators simply offer a % of their royalties to marketplaces.

Example: If collection XYZ decides to collect 5% royalties, they may elect to give a quarter of those royalties to the marketplace that led to that transaction. The marketplace would be rewarded 1.25% of the total transaction.

## Standardization

A standard royalty protects collectors. A standard reward protects marketplaces.

Creators should agree on a standard royalty % (we suggest 5%)
Creators/marketplaces should agree on a standard marketplace reward (we suggest 25% of collected royalties)

What stops creators from setting a 0% reward for marketplaces? You can expect a marketplace not to list your NFT if your rewards aren't meeting their standards.

## Other proposed solutions

### Operator Filters

Blocklists are going to be a pain to maintain. And do you *really* want to turst one of the existing marketplaces to maintain it for you? They may choose to block any marketplace for *any* reason and penalize anyone who doesn't play ball.

### A DAO

If a DAO is in charge of an allowlist of royalty-enforcing marketplaces, it'll be a pain for any new marketplace to get on the list. *Marketplace makers are also creators*, so let's empower the best creators to create amazing marketplaces without more barriers to entry!

### Workarounds

Anyone can create a false "marketplace" to collect the reward.

## Restrictions

In order to prevent marketplaces from trading a collection the way they do today (for 0% royalties), restrictions would be placed on the existing `approvalForAll` and `approval` functions.

## What this doesn't solve

Unfortunately, this doesn't solve the immediate problem: existing, non-upgradeable contracts. Unfortunately, it's been hard to find a good solution to enforce royalties for this. Asking a marketplace to honor royalties is also asking them to slowly bleed. If that marketplace folds, what happens next? All collectors will migrate to the marketplaces that do not honor royalties.

This is the miserable cost of being first to market, but we're hoping a new solution blooms for legacy collections.

## Credit

* xtremetom independently came up with a similar solution, and we spoke to hash out some details
* Satoshi Nakajima wrote a [proposal](https://hackmd.io/@snakajima/BJqG3fkSo) which sparked the initial exploration
