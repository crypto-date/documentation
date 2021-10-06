# Tokenomics

### Total Possible Supply Of Cryptodate NFTs

There are 100 years of NFTs available. Accounting for leap years, the total possible number of cryptodate NFTs that can be minted is **36,525 NFTs**.

  ***(366 * 25) + (365 * 75) = 36,525***

| Type | Price | Supply | Formula | Comment |
| :--- | :--- |  :--- | :--- | :--- |
| Exclusive | Base Price * 100 | 25 | Each leap day | The 29th day of each leap year, e.g. Feb 29 2000 |
| Limited | Base Price * 10  | 1,200 | Each day that matches month | When the number of the day and month match, e.g. Mar 3, April 4, etc. |
| Standard | Base Price | 35,300 | All remaining days | From Jan 1 1950 to Dec 31 2049, excluding the dates above |
| **Total** |  | **36,525** | **All days** | **From Jan 1 1950 to Dec 31 2049** |

### Price of Cryptodate NFTs

The initial base price of a cryptodate will be .1 ETH/BNB. This base price may change as the market determines the floor. The current base price can always be found by querying the smart contract. Given this initial base price, the total initial value of cryptodates can be calculated:

| Price | Supply | Value |  
| :--- | :--- | :--- |
| 10 ETH/BNB | 25 | 250 ETH/BNB |
| 1 ETH/BNB | 1,200 | 1,200 ETH/BNB | 
| .1 ETH/BNB | 35,300 | 3,530 ETH/BNB | 
| **Total** | **36,525** | **4,980 ETH/BNB** | 

There is an ability to change the base price through governance. The long term plan is to fix the base price and renounce the ability to change it forever. 

### Cryptodate Token \(CDT\) Distribution on Ethereum

The initial value of CDT will be set to mimic 1 USD. However, this is not a peg and fluctuate with supply/demand of cryptodates. 

The distribution of CDT has been designed given the above initial price calculation such that sufficient CDT is locked in smart contracts for the purpose of minting rewards, ownership rewards and automated liquidity provisioning.

| Purpose | Number of Tokens | Percent | Location | Comment |
| :--- | :--- | :--- | :--- |  :--- |
| Minting & Ownership Rewards | 12,000,000 | 40% | Locked in NFT smart contract | Sufficient for minting rewards and ownership rewards of 100 CDT per NFT for 3 years.  |
| Automated Liquidity Provisioning | 6,000,000 | 20% | Locked in NFT smart contract | Sufficient to supply AMM upon minting NFTs. |
| Staking & Liquidity Rewards | 6,000,000 | 20% | Locked in staking smart contracts | Sufficient for multiple reward periods to incentivize holding CDT. |
| Commissions, Marketing, Operations| 6,000,000 | 20% | Held by treasury | Allocated to spend on art through community commissions, marketing and operational costs. |
| **Total** | **30,000,000** | **100%** |  |  | |



