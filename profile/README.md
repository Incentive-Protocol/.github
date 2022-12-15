# Incentive Protocol 
![](https://i.imgur.com/UaNSxKi.png) 

The logo represents multiple parts that cooperate to create a strong force, the more parts join, the bigger the impact. 


## 🖋️ Introduction 
One day we got bored of the user experience in a restaurant... long wait just to receive the menu, trying to figure out how some dishes could look like from the description and not so much flexible payment options. 

So we started to think about how we could use technology to create a better user experience, both for the customer and the restaurant. 

This is where we conceptualised Incentive Protocol, an **open-source** protocol that connect businesses and customers, offering multiple features able to drastically  improve restaurant performance. 

Incentive Protocol first [whitepaper](https://docs.google.com/document/d/1koxsNgYxQWTPLAFO-CNTEHkeTCfIwqkRtGIJcuud8BQ/edit?usp=sharing). 

## 📜 Principles
Here some principles we believe in
- Open-source infrastructure. 
- Collaboration: anyone is free to download the code and cooperate. Together we are stronger. 
- Open-mindset: we are open to also different implementations of the architecture, as long as we can achieve the same goals. 
- Decentralized: no central parties should handle payments, that's why we use blockchain technology. 
- Self-custody: user and businesses should be able to truly own their funds. 
- Collaborative data sharing: combining and sharing data gathered on top of the protocol. 
- Privacy: user who want to should be able to preserve their privacy and protect their identity. 
- Permissionless: anyone following the rules should be able to partecipate and build on top of the protocol. 

## ⚙️ How Incentive works? 
### 🔗 First layer 
A collection of smart contracts that are mainly responsible for
- user account generation: anyone can choose from two type of accounts: seller account and the buyer account. 
-- The seller account (for businesses) can create what we call incentives. 
-- The buyer account can mainly buy incentives from sellers. 
- An incentive is the process of posting a product with his relative information, like description, category and price, with multiple price mechanism. 
- In our design, an Incentive it's an non-fungible-token, it can act like a receipt or even an access to products and services.
- Mapping existing accounts with their respective informations. 

### 📱 Application layer 
On the application layer, anyone can build a front-end that communicate with Incentive main smart contracts.

We believe that the UI/UX should be simple and easy to use, so anyone can benefit from the technology. Without goint far from the first principles, like self-custody and decentralized payments. 

A good UI/UX is not just about the easiness of the platform, but also the account creation process and the payment flow, it should be quick as traditional web2 infrastructures. 

We as Incentive Labs will build 
- a platform to facilitate the search and purchase of incentives. 
- On the same platform user and businesses can create and manage their accounts, using even traditional methods like social logins powered by AuthO. 
- It's important to have accounts decentralized as possible, for this we will use existing platforms like [Web3auth](https://web3auth.io/) or [Magic.Link](https://magic.link/). They use different implementations of threeshold cryptography to distribute private keys to multiple parties. I wrote a [note](https://arc.net/p/F217C635-6ABF-4410-80CE-02A3D4AB61B1) on why traditional self-custody is hard.
- Using these technologies we can power payments both with FIAT and Cryptocurrencies. 

## 🤔 Some technical considerations

The smart contract need cryptocurrencies to process payments, so the payment process is about converting FIAT into cryptocurrencies, and then use cryptocurrencies to finalize the payment. This method is referred as [ON-RAMP](https://coinmarketcap.com/alexandria/glossary/fiat-on-ramp). This whole process it has to happen in a few seconds. 

Users should be able to also deposit into the wallet easily with multiple methods, like credit and debit cards, bank transfers and open-banking systems. 

Businesses should be able to withdraw easily. In a typical process a business need to open an account with a centralized exchange like Binance or Coinbase, send their funds to that exchange, convert the cryptocurrencies to FIAT, and finally withdraw. There are too many steps involved. 

So in our implementation, we will use a process in which a business withdraw by selling directly the received cryptocurrencies into FIAT from the web-app, a process called [OFF-RAMP](https://www.hydrogenplatform.com/blog/what-does-crypto-on-ramp-and-off-ramp-mean#:~:text=Off%2Dramping%20refers%20to%20the,service%20directly%20with%20your%20crypto.). 

Using a mix of ON-RAMP and OFF-RAMP we can create a smooth user experience, from the purchase to the withdrawal, in the most decentralized way, with instant liquidity for the businesses. 

If you ever run a business online, at some point you surely experienced long waits just to receive your funds from platforms like Paypal. In some case some businesses got their funds [held](https://www.dailydot.com/debug/paypal-withholding-funds-small-business/) for months without a valid explanation. 

So it's pretty explanatory why businesses should own their funds. 

## 🛢️ Open database
The idea is to collect any relevant data on an open database that can be queried by any developer bulding on top of Incentive protocol. 

The database choice should be an open-source infrastracture that have fast read operations to deliver performant dApps (decentralized apps). 

An example could be a platform that show detailed reports about sales for businesses. The front-end could query our database to generate graphs and businesses could access using their universal account. The platform could even charge for this additional service. We could see [SaaS](https://digitalguardian.com/blog/what-saas-company) businesses built on top of the protocol. 

A shared database could also mean better data collection, single businesses haven't enough data to offer meaningful services like product recommendation, but if they could benefit from each other data, we could offer powerful services. 

We all know that big corporations like Amazon, Netflix are so good because they can collect a huge amount of data that they can use to offer better services. 

This could be the first example of single businesses indirectly partnering to better serve their customer. 

We incourage you to suggest us the best choice we could make for the database infrastructure. 

## 💡 Other ideas 
Here a list of features we would like to implement, we invite anyone with the right expertise to help us implement some of the things listed. 

- What if the application could suggest you new dishes based on your past transactions? That could be done with two ways, the first could be done with [collaborative filtering](https://developers.google.com/machine-learning/recommendation/collaborative/basics), and a second new approach from OpenAI would be using [CLIP](https://openai.com/blog/clip/), an approach that use neural networks, withouth the need to use image metadata.  
-- While collaborative filtering has beend used with great success, Clip approach looks pretty interesting
![](https://i.imgur.com/F4jmALA.jpg) Image from OpenAI.


