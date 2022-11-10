# ERC-721ROY

The best builders in the metaverse support creator royalties. The wisest ones will reward marketplaces that also support royalties. This symbiotic relationship is crucial for the health of the metaverse.

Introducing ERC-721ROY, a new standard that enforces royalties while rewarding marketplaces.

## Basic Functions

New functions in ERC-721 that enable…
* a token owner to list their token(s) for sale on contract
* a collector to buy tokens on contract
* a contract owner to collect royalties on sales

## Benefits

* No third party required to sell an NFT
* Listed NFTs automatically appear on *all* marketplaces that support this standard
* Set `approvalForAll` is no longer needed, reducing scams (scammers are trash 🤮)
* Bulk listing/buying means gas savings

## Additional Functions

Additional features would allow…
* a collector to bid on an NFT/collection by staking their eth
* a token owner to accept a bid
* a contract owner to reward marketplaces a % of collected royalties

And of course, a way to remove all your listings/bids

## Incentivizing Marketplace Development

NFT creators need to incentivize marketplaces to list their collection. This is simple: creators will offer a % of their royalties to marketplaces.

Example: If collection XYZ decides to collect 5% royalties, they may elect to give a quarter of those royalties to the marketplace that facilitated that transaction. The marketplace would be rewarded 1.25% of the total transaction while the creator keeps 3.75%.

With rewards, marketplaces will compete to craft a great experience for collectors. (Yes, marketplace creators are creators, too.)

## Standardization

A standard royalty protects creators & collectors. A standard reward protects marketplaces.

NFT Creators should agree on a standard royalty (we suggest 5%).
NFT Creators/marketplaces should agree on a standard marketplace reward (we suggest 25% of collected royalties).

What stops creators from setting a 0% reward for marketplaces? You can expect a marketplace not to list your NFT if your rewards aren't meeting the standard.

## Other proposed solutions

### Operator Filters

Blocklists are going to be a pain to maintain. Plus, do you *really* want to trust an existing marketplace to maintain that list for you? They may block *any* marketplace for *any* reason and penalize *anyone* who doesn't play ball.

### A DAO

A DAO can continually curate an allowlist of royalty-enforcing marketplaces. However, members of the DAO often stop voting, and a powerful marketplace can gain a sizeable share of the DAO, defeating its purpose. In addition, creators building new marketplaces would have an additional barrier to entry since they have to be approved by the DAO.

## Workarounds to ERC-721ROY

* Anyone can create a false "marketplace" to collect the reward. Creators of this false marketplace generally wouldn't share it with the rest of the public.
* Tokens can be wrapped and transacted the old way. However, this creates friction that the general public would rather avoid.

## Restrictions

In order to prevent marketplaces from trading a collection the way they do today (for 0% royalties), restrictions would be placed on the existing `approvalForAll` and `approval` functions.

## What this doesn't solve

Unfortunately, this doesn't solve the immediate problem: existing, non-upgradeable contracts. Unfortunately, it's been hard to find a good solution to enforce royalties for this. Asking a marketplace to honor royalties is also asking them to slowly bleed. If bleeding causes that marketplace folds, collectors will migrate to the marketplaces that do not honor royalties.

This is the unfortunate cost of being first to market, but we're hoping a new solution blooms for legacy collections.

## Credit

* xtremetom independently came up with a similar solution, and we spoke to hash out some details
* Satoshi Nakajima wrote a [proposal](https://hackmd.io/@snakajima/BJqG3fkSo) which sparked the initial exploration
