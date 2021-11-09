# Christmas Tree Generative Art Collection #

 The Cryptodate Christmas tree collection represents each Christmas Day from 1950 - 2049 as a unique PNG image of a generated Christmas tree. The collections can be found here:

* [Ethereum](https://www.cryptodate.io/eth/collection/xmas_tree)
* [BSC](https://www.cryptodate.io/bsc/collection/xmas_tree)
* [Polygon](https://www.cryptodate.io/polygon/collection/xmas_tree)

 
 To generate the image, Christmas tree "DNA", stored on chain, is used to determine how the tree looks. Each tree has a unique background color and the following possible traits:

 * Gifts
 * Star
 * Garland
 * Ornaments
 * Lights

The "recipe" for generating a tree is explained below. Thus, each tree can be rebuilt, Sol de Witt style. 

## DNA ##

A tree's DNA is formulated by taking the token id of the tree (aka **19501225**) plus the network the tree was minted (aka **eth**) and creating its MD5 hash. (The token id is always on Christmas day.) 

In Javascript, the code looks like this  although any programming language will make the same DNA:

``` javascript
const dna = md5("19501225_eth");

```

For example, MD5 hash of **19501225_eth** is **21a6cdf7214d121b2423d8b7e1efe70e**. We now have the tree's DNA. 

Only the first 11 characters of the DNA is used:

* Characters 0-5 are used to determine the background color. In the example above, the background color would be **#21a6cd** from the DNA **21a6cd**f7214d121b2423d8b7e1efe70e. 
* Characters 6-10 are used to determine which traits the tree has, based on whether the character is a number or letter. Since there are 10 possible numbers and 6 possible letters a trait's slot, it means that traits are either %37.5 likely, or %62.5 likely. As such, the algorithm make gifts, stars and garlands only %37.5 likely to appear on a tree, but ornaments and lights are  %62.5 likely. 

As such, certain combinations are more rare and a tree with all traits is very uncommon!

For example, in the case above, the trait DNA is **f7214** from the DNA 21a6cd**f7214**d121b2423d8b7e1efe70e. That means it has gifts (**f**), but no star (**7**), and no garland (**2**). It does have  ornaments (**1**) and lights (**4**).

Here's the algorithm in Javascript. It could easily be recreated in any language:

```javascript

const color = dna.slice(0,6);
const chars: string[] = dna.split("");
let traits: string = "";
Number.isNaN(+chars[6]) ? traits = traits + "traits/gift.png " : "";
Number.isNaN(+chars[7]) ? traits = traits + "traits/star.png " : "";
Number.isNaN(+chars[8]) ? traits = traits + "traits/garland.png " : "";
!Number.isNaN(+chars[9]) ? traits = traits + "traits/ornaments.png " : "";
!Number.isNaN(+chars[10]) ? traits = traits + "traits/lights.png " : "";

```

Once the traits are determined, Imagemagick is used to layer the transparent PNGs into the final tree:

```javascript 

            const args = `convert -background "#${color}"  traits/Base.png ${traits} -flatten -bordercolor "black" -border 20 trees/${network}/${date.getFullYear()}1225.png`;
            
```


## Assets ##
All assets for generating the trees can be downloaded here:

![Alt text](https://assets.cryptodate.io/eth/dynamic/19701225.png "Logo")

