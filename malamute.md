# Alaskan Malamute Generative Art Collection #

 The Alaskan malamute collection generates a unique malamute for each Malamute day (January 7th). The collections can be seen here:

* [Ethereum](https://www.cryptodate.io/eth/collection/malamute)
* [BSC](https://www.cryptodate.io/bsc/collection/malamute)
* [Polygon](https://www.cryptodate.io/polygon/collection/malamute)
* [Avalanche](https://www.cryptodate.io/avax/collection/malamute)
* [Fantom](https://www.cryptodate.io/fantom/collection/malamute)
* [Moon River](https://www.cryptodate.io/movr/collection/malamute)

 
 To generate the image, malamute "DNA", stored on chain, is used to determine how the dog looks. Each dog has a unique background color and the following possible traits:

 * Fur
 * Eyes
 * Hat
 * Mouth
 * Shirt

The "recipe" for generating a dog is explained below. Thus, each dog can be rebuilt, Sol LeWitt style. 

## DNA ##

A tree's DNA is formulated by taking the token id of the tree (aka **19500107**) plus the network the tree was minted (aka **eth**) and creating its MD5 hash. (The token id is always on January 7th.) 

In Javascript, the code looks like this  although any programming language will make the same DNA:

``` javascript
const dna = md5("19500107_eth");

```

For example, MD5 hash of **19500107_eth** is **dd9eb6bfc1e964d169c17c35ea956a6d**. We now have the dog's DNA. 

Only the first 6 characters of the DNA is used:

* Character 1 is used to determine the background color
* Character 2 is used to determine the fur color
* Character 3 is used to determine the eyes
* Character 4 is used to determine the hat, if any
* Character 5 is used to determine the mouth
* Character 6 is used to determine the shirt, if any

As such, certain combinations are more rare and a dog with all or no traits is very uncommon!


![Alt text](https://assets.cryptodate.io/bsc/malamute/19830107.png "Logo")

