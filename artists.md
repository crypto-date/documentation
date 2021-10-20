# A Different Kind Of Minting Platform

The token id of most NFT projects has no semantic value. It simply creates a unique id that, when paired with a contract address, serves to identify the NFT. Ultimately, it is the tokenURI that points to the metadata about the NFT which most users are interested in.

The cryptodate system is different. The token id has semantic meaning: it is the date that the user is buying. As such, owning a cryptodate means you own the data on-chain and that date is immutable. 

The cryptodate NFT smart contract does support off-chain metadata.  Each cryptodate NFT points to a tokenURI. The metadata discovered in that tokenURI includes a link to an image stored on a server. By default, all cryptodates have dynamic art generated as an .svg. But, the link to that default image can be updated to point to a different image. 

In this way, an artist can create new art for a token id **before** the NFT is minted, overriding the default .svg image. Additionally, an owner of an NFT can create new art for a token id **after** the NFT is minted, through a process using cryptographic signatures and spending CDT utility tokens.

This novel minting system uniquely takes advantage of the ERC721 specification by combining the best of mutable and immutable data. 

### Example 1

An artist could be commissioned to create a piece for a token id, say January 1, 2001 or **20010101**, that has not been minted. The artist would be paid for this commission in CDT tokens and the art itself would be uploaded to a server. The image url for **20010101** would be updated to that URL. If the art sold, the proceeds would immediately increase the value and liquidity of CDT. 

### Example 2

An collector could mint his/her child's birthday, say April 21, 1996 or **19960421**. He/she could then cryptographically validate that they are the owner of that date and upload a painting of their child to a public url. He/she could then spend CDT tokens for the privilege of updating the metadata for that token to the new image URL.

## Commission Process

If an artist is interested in designing a piece for the cryptodate system, they can make a proposal which will be voted on via governance. If approved, they will be allocated the CDT tokens upon completion of the art.

## Updating Metadata After Minting

See the roadmap for when this will be available.

