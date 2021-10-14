# Cryptodate NFTs 

## Properties

Cryptodates are non fungible tokens representing a unique day from January 1, 1950 to December 31, 2049.  The date itself is represented on chain as the token id of the NFT, formatted  as **yyyymmdd**. For example, the day January 1, 2001 would be formatted **20010101**.

Cryptodates are fully compliant with the ERC721 specification, including the enumerable addendum.  As such, they can participate in any part of the ERC721 ecosystem.

Cryptodates are not burnable. 

## Metadata
Cryptodates have external metadata pointing to a templated, unique art formatted as .svg.  Some dates have overridden the default template with art. This art (.png, .svg or .mp4) may be linked to a single cryptodate or it may have multiple editions. As time goes on, more NFTs with unique art will be created. 

## Cryptodate Pricing

Cryptodates have a base price. Certain dates are algorithmically established to cost a factor greater than the base price:

| Type | Price | Quantity | Formula | Comment |
| :--- | :--- |  :--- | :--- | :--- |
| Exclusive | Base Price * 100 | 25 | Each leap day | The 29th day of each leap year, e.g. Feb 29 2000 |
| Limited | Base Price * 10  | 1,200 | Each day that matches month | When the number of the day and month match, e.g. Mar 3, 1998 |
| Standard | Base Price | 35,300 | All remaining days | From Jan 1 1950 to Dec 31 2049, excluding the dates above |

## Cryptodate Bonus

Whenever a cryptodate is minted by a collector, the buyer is immediately rewarded a bonus of cryptodate tokens (CDT). The amount of the bonus is based on the price * 100. So, if the base price was .06 ETH, a bonus of 6 CDT would be paid out immediately upon purchasing a standard NFT, 60 CDT for a limited NFT and 600 for an exclusive NFT. 

## Cryptodate Ownership Rewards

Cryptodates have the unique property of earning CDT simply by owning them. This yield is set as a fixed interest rate of 100 CDT per cryptodate per year. This rate cannot fluctuate and is baked into the smart contract. The smart contract is funded to provide this fixed rate for 3 years. Rewards could run longer if not all cryptodates are minted within the first year.

If a person relinquishes ownership of a cryptodate by gifting or selling that date, the interest accrued on that date up to the moment of transfer is still held by the original owner. As such, one doesn't have to remember to claim the interest on a date before selling it.

The new owner will begin earning interest upon transfer.

Yield can be withdrawn at any time. 


