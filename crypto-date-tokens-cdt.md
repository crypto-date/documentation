# Cryptodate Tokens \(CDT\)

The cryptodate token \(CDT\) is an ERC20 compliant token for the purpose of governance of the cryptodate system as well as for various utilities when using the system.  \(See [Governance](governance.md) for more.\) Tokens can be earned by using the system itself:

* Minting rewards for buying a cryptodate
* Ownership rewards for holding a cryptodate
* Rewards for providing liquidity to the CDT/ETH pool
* Rewards for staking CDT
* Creating art for a set of dates

See [Tokenomics](tokenomics.md) for exact token amount allocations.

## Minting Rewards

Whenever a date is minted in ETH, a one time reward of CDT is automatically transferred to the minter based on the price paid for the NFT. This formula is calculated as 100x the price paid.

If the price of a  cryptodate in is **.1 ETH** a reward of **10** CDT would be issued. 

## Ownership Rewards

Cryptodates have the unique property of earning CDT simply by owning them. This yield is set as a fixed interest rate of 100 CDT per cryptodate per year. This rate cannot fluctuate and is baked into the smart contract. The smart contract is funded to provide this fixed rate for 3 years.

## Liquidity Provider Rewards

If a person adds liquidity to the ETH/CDT liquidity pool (either on Uniswap v2 or Pancakeswap), he/she can earn rewards by staking those LP tokens.  Adding liquidity incurs the standard risks of impermanent loss that all pools incur. Since the smart contract itself uses the pool, there are guaranteed fees generated from the pool.

## Staking Rewards

Rewards can also be earned by staking CDT in the staking contract. 

