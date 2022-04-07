# Zoubair HATTAB  

## fractionalNFT.sol
Visit the Remix IDE or use Truffle on VSC . Then copy and paste the fractionalNFT.sol source code. then Compile  && Deploy .
before we can mint the NFT, we must store its title deed permanently we con use ipfs could .

At the mint command of fractionalNFT.sol, the Property Owner enters the following:
1. to: the property owner’s wallet address
2. tokenURI_: the CID link to the title deed that we have copied from IPFS
3. _totalFractionalTokens: number of the fraction NFT for example 1 milion ERC20 

## Fractional Tokens
The fractionalNFT.sol smart contract maintains a mapping that associates the FNFT NFT token with its FNT tokens. To view it, 
enter the token ID at the FNFT function. Click [Call] to view the address of the FNT tokens.
Copy the address.
then you should be   Change the contract to FNFToken at REMIX. Then paste the address that you have copied in the previous set to “At Address”.
To view the total token supply of the FNT tokens,click on the function  totalSupply you will the number of the fraction ERC20.
##   Fractional Claim contract .
the reason to create this contract for example if the owner of NFT wants to sell this NFT to another owner.
but he has co-owners in this NFT  like shares of ERC20 . the problem here no buyer will accept to buy this NFT  because if he buys this from the owner he will inherit it with another co-owners.
in this case, the owner NFT wants to sell this NFT should be taken agreement from the co-owner before all things and he will pay every co-owners to buy his fraction of ERC20.
Visit the Remix IDE or use Truffle on VSC . Then copy and paste the fractionClaim.sol source code. then Compile  .
## Deploy Fractional Claim contract

Enter the Fractional NFT Smart Contract Address and the Token ID representing the property. Click transact this i'm using REMIX .

## Redeeming fraction ERC20 Tokens to the owner NFT

each Fractional Owner must first give permission to the Fractional Claims Smart Contract to interact with his FNT Token.
He goes to the FNT Token Smart Contract and enters the Fractional Claims Smart Contract address. He also enters the total amount of FNT tokens that he will be redeeming.
At the Fractional Claims Smart Contract, he enters the Smart Contract address of the FNT token and the amount that he is redeeming.
The Fractional Claims Smart Contract takes his FNT tokens and burns them. It calculates the total ETH that he is entitled to and sends it to him.
after this each Fractional Owner will redeeming ETH will burn this fraction 

