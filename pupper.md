# Crypto Pupper Generative Art Collection #

 The Crypto Pupper collection generates a unique pupper for each Puppy day (March 23rd). The collections can be seen here:

* [Ethereum](https://www.cryptodate.io/eth/collection/pupper)
* [BSC](https://www.cryptodate.io/bsc/collection/pupper)
* [Polygon](https://www.cryptodate.io/polygon/collection/pupper)
* [Avalanche](https://www.cryptodate.io/avax/collection/pupper)
* [Fantom](https://www.cryptodate.io/fantom/collection/pupper)
* [Moon River](https://www.cryptodate.io/movr/collection/pupper)

 
 To generate the image, pupper "DNA", stored on chain, is used to determine how the pupper looks. Each pupper has a unique background color and the following possible traits:

 * Fur
 * Eyes
 * Hat
 * Mouth
 * Shirt

The "recipe" for generating a pupper is explained below. Thus, each pupper can be rebuilt, Sol LeWitt style. 

## DNA ##

A tree's DNA is formulated by taking the token id of the tree (aka **19500323**) plus the network the tree was minted (aka **eth**) and creating its MD5 hash. (The token id is always on March 23rd.) 

In Javascript, the code looks like this  although any programming language will make the same DNA:

``` javascript
const dna = md5("19500323_eth");

```

For example, MD5 hash of **19500323_eth** is **13ec293c4dae36c500f4a8d64351d5d7**. We now have the dog's DNA. 

Only the first 6 characters of the DNA is used:

* Character 1 is used to determine the background color
* Character 2 is used to determine the fur color
* Character 3 is used to determine the eyes
* Character 4 is used to determine the hat, if any
* Character 5 is used to determine the mouth
* Character 6 is used to determine the shirt, if any

As such, certain combinations are more rare and a pupper with all or no traits is very uncommon!


![Alt text](https://assets.cryptodate.io/avax/pupper/19830323.png "Logo")

