# Decentralize Centralized Crypto Exchanges  Proposal v1

**August 01, 2019**

**Abstract:** This system is meant to build up a decentralized system to make use of existing centralized cryptocurrency exchanges to make people ( we call them 'trader' in the subsequent proposal ) trade crypto in a convenient and secure way.  People don't need to sign up in any crypto exchanges in order to trade cryptocurrencies.  Others ( we call them 'relay' in the subsequent proposal ) who has accounts in any crypto exchanges can act as an intermediate to relay orders to different exchanges. Smart contract based on existing blockchain is used to guarantee a trustless and secure trading environment for traders and relays.  This system also designs an appealing incentive mechanism to attract people to act as the relays. 



Copyright © 2019

**DISCLAIMER:** Without permission, anyone may use, reproduce or distribute any material in this proposal for non-commercial and educational use (i.e., other than for a fee or for commercial purposes) provided that the original source and the applicable copyright notice are cited.



- Background

- Requirements

  - easy for use
  - advance the universal Authentication
  - smart contract to guarantee safety and security  for both traders and relays
  - incentive mechanism to attract relays to pour liquidity into the system
  - integrated depth for people to view crypto market in different exchanges

- General proposal

  - Buy process
  - Sell process
  - Incentive mechanism

- Conclusion

  ​

# Background

After I presented the 'Crypto Exchanges Integration' in hackathon in my company,  lots of colleagues asked me how to sign up in any exchanges, how to pick up exchanges, they have no idea where to buy and sell cryptocurrencies and how.  Some colleagues are  professional at trading in the market, but they feel uncomfortable due to the low liquidity in current cryptocurrency market.  After talking with some brokers, actually none of those traditional brokers are likely to take this system due to unclear regulations.



In addition, I once used some decentralized cryptocurrency exchanges, however, most of them can only trade tokens based on the same blockchain ecosystem and most of them lack of enough liquidity, which scare people off.  In contrast,  many centralized crypto exchanges have lots of liquidity and people can trade different pairs of cryptocurrencies, tokens. However, these centralized exchanges are often hacked or cheat their clients.  We cannot expect a single broker to take all those risks. 



OTC ( Off-The-Account ) trading is another nightmare for traders especially buyers.  First of all, in most time, buy price is far from the fair market price, so buyers need to overpay to get the ownership of a crypto. Second of all, there is few brokers who can offer coins, it is impossible to purchase a large amount of coins. At last, they are still centralized system and clients are under the risk of being hacked or cheated.



This triggered my interest to build a decentralized system to make use of  these centralized exchanges which spread all over the world.  If I want to place an order to buy or sell, I don't need to sign up in any exchanges to submit my personal information many times. When I want to place an order for a pair of cryptocurrencies, my order can be taken by unknown people and flow into different crypto exchanges, once filled, I can get cryptocurrencies into my private wallet.   For people act as relays, they can find orders in the market and get it filled so that they can win some rewards.  Blockchain and its smart contract is just right for this system to guarantee safety and secure trading, as well as offer incentive mechanism to attract enough liquidity to this system.



# Requirements

In order to gain widespread use, this system requires a platform that is flexible enough to meet the following requirements:

## easy for use 

People who use this system don't need particular knowledge of cryptocurrency exchanges or private/public key. This requires the system can automatically integrated with clients' own wallets.  For relays, it does't need professional technical knowledge to take orders and relay to exchanges they signed up with. Stable coin is a very important concept in this system. With the development of Facebook Libra, 

## advance the universal Authentication

This application should  support a myriad of Authenticators used to access transactions. There should be complete clear authorization before placing orders.

## smart contract to guarantee safety and security  for both traders and relays

Smart contract over existing blockchain such as EOS and ETHEREUM is the best way to ensure the security and safety of both traders and relays.  Various ways to attack the contract should be considered and prevented.

## incentive mechanism to attract relays to pour liquidity into the system

There should be incentive to attract people to relay orders, they should get rewarded from the system so that they can be stimulated to introduce liquidity from centralized exchanges. 



## integrated depth for people to view crypto market in different exchanges

The system will provide integrated depth view for some crypto exchanges so that both traders and relays can have a rough knowledge what the current market price is for pair coins.





# General proposal

For authentication, we will try to use existing mature modules instead building wheels from scratch. A draft buy and sell processes are illustrated:

## buy process

e.g. Alice wants to buy in 10 BTC, however, she doesn’t have any accounts in any crypto exchanges.  Jessie has signed up in BTCMarket, Jerry has signed up in coinbase, Tom has signed up in binance. Alice wants to buy in with price 9300 USD, she sends 9300X10 USD ( stable coins such as USDT, DAI, TUSD or Libra ) to a smart contract in Ethereum  or EOS  and sends her order.

The system has a price feed to scan market data from many crypto exchanges and this is visible to all people. Tom sees this order can be partially filled in binance so he takes the order and relay it to binance.

Jerry relays part of the volume to coinbase and Jessie relays to BTCMarket.



![img](https://miro.medium.com/max/640/0*pfvACHXFXtXqftZo.png)



Once the orders get filled, Tom, Jerry and Jessie will send BTC to Alice’s wallet address, once this is confirmed by Alice or the time is up, the smart contract will release stable USD coins to Tom, Jerry and Jessie’s accounts. After deduction of commission fee and transfer fee, the surplus is returned to Alice’s account. Tom, Jerry and Jessie will be rewarded by smart contract accordingly.





## sell process

The sell process is somehow like this: Alice wants to sell 10 BTC, so she places this order. To save transfer fee, she can send the order in ‘fill or kill’ mode so that that order won’t be split into small ones, or she can let it be so that order can be taken by different people. Tom will deposit some stable coins to the smart contract and 3 BTC will be sent to Tom’s address and then he can either sell his own BTC to binance or wait until Alice’s BTC arrives his account then sell it. Jerry can do the same and sell order to coinbase. Jessie can sell part of the order to BTCMarket. On the settlement, Tom, Jerry and Jessie will send message to smart contract on how many volumes have been filled. The smart contract will ask them to return part of the BTC to Tom’s account, once this is confirmed or time up, the smart contract will release stable coins to Alice’s account based on how many BTC has been traded and return surplus to Tom, Jerry and Jessie after taking commission and transfer fees. Tom, Jerry and Jessie will be rewarded by smart contract accordingly.



![img](https://miro.medium.com/max/640/0*Y7LgxNfQd6Ix75Sn.png)



The stable coin is very important in this system and to make things easy, we can use the existing stable coins such as USDT, GUSD, PAX which compliant to ERC20 if this system is running in Ethereum, or other stable coins based on EOS if this system will run on EOS.

Assumption: there are convenient ways for ordinary people to obtain stable coins by trading with fiat currency, with the Libra issued by Facebook and more governments, companies issuing their stable coins, this is becoming much more realistic and convenient.



## incentive mechanism

- each time a transaction is completed, people who relay orders will be rewarded with ‘DCI’;

- ‘DCI’ is produced in the way only when a transaction happens after the system launches;

- when a transaction is completed, there will be commission fee debited from traders, this fee will be kept in the smart contract and send to ‘DCI’ holders regularly;

- ‘DCI’ holders are responsible for the vote for proposals such as proportion rewarded to brokers and how smart contract should work to maintain the community, what stable coins should be included in the system.

  ​




## Conclusion

This system is an excellent usage of smart contract in blockchain to secure traders and relays in a trustless way.  With stable coins, incentive mechanism introduced, it can facilitate buyers and sellers in the cryptocurrency world by make use of liquidity centralized exchanges, even extends to decentralized exchanges.  It can benefit not only traders, but also all the ecosystem in the blockchain and cryptocurrency.    Either Ethereum or EOS should make use of this De-Finance system to strengthen its community.  

