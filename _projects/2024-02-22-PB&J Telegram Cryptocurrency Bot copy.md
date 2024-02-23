---
layout: projects
author: Tommy
desc: A PB&J storefront project built on telegram powered by python-telegram-bot library using Bitcoin for transactions.
project_date: November 2023 - Present
---
# PB&J Telegram-Cryptocurrency-Bot
A storefront project built on telegram powered by python-telegram-bot library using Bitcoin for transactions.

The bot features a clickable chat menu for all the goods and information that a PB&J enjoyer might find useful.


### Purpose
- The project is a fully functional storefront, that sells... PB&Js for Bitcoin!
   - Offers a wide variety of PB&J items with different bread combinations
        - White Bread
        - Whole Wheat
        - Honey Wheat

![Telegram Screenshot of Main Menu]({{site.baseurl}}/assets/images/Telegram-MainMenu_Screenshot.PNG){: .img-fluid .screenshot .shadow-lg}
![Telegram Screenshot of Main Menu]({{site.baseurl}}/assets/images/Telegram-PB&J_Screenshot.PNG){: .img-fluid .screenshot .shadow-lg}
![Telegram Screenshot of Main Menu]({{site.baseurl}}/assets/images/Telegram-PB&J_Cart_Screenshot.PNG){: .img-fluid .screenshot .shadow-lg}
![Telegram Screenshot of Main Menu]({{site.baseurl}}/assets/images/Telegram-Checkout_Screenshot.PNG){: .img-fluid .screenshot .shadow-lg}
![Telegram Screenshot of DB in React]({{site.baseurl}}/assets/images/React_PB&J_Orders.PNG){: .img-fluid .screenshot .shadow-lg}
![Telegram Screenshot of DB in React]({{site.baseurl}}/assets/images/React_PB&J_Cart.PNG){: .img-fluid .screenshot .shadow-lg}
![Telegram Screenshot of DB in React]({{site.baseurl}}/assets/images/React_PB&J_Users.PNG){: .img-fluid .screenshot .shadow-lg}
#### Current Capabilities
- Able to order any item with any bread with any quantity
- Generates Satoshi amount for a USD equivalent on real-time market
- View MongoDB data on a React Webpage
- Modify any data on React datatables 
- Stores information on user activity (buttons pressed, last active, etc.)
- Retains user chat and cart state between sessions
{.paper}

### Technologies/Tools Involved
- AWS EC2 (Hosting the Telegram Bot)
- MongoDB Atlas (Powers the database)
- Vercel (Next.js host)
- Python-Telegram-Bot (Library for interacting with Telegram)
- Bit (Calculates the USD -> Bitcoin Rate and other bitcoin transactions)
- ReactJS (Used for creating a dashboard/table for viewing database)

## Project Challenges
##### Anonymity 
Anonymity is a large reason as to why bitcoin is so powerful. I wanted to protect a users anonymity and make those users feel more secure while they are using my store. A darkweb website prevents an average user from even approaching based on stigmas associated with the darkweb.

This has a couple implications.
- Transactions can be traced when using a bank card
- Users can still be releasing data on their own accord through account metadata
- Users transactions might be intercepted by third-parties
- Users need to feel secure, but might not actually be the most secured

Telegram offers API for interacting with their bot chats, encrypted chats, and is a very popular tool for discrete conversations.

##### Telegram
Telegram provides an HTTP API that can be used with a lot of customizability. I wanted to get this project running without having to deep dive into the boilerplate code and was willing to trade off some of the customizability associated.

I chose python-telegram-bot library for its simplicity and representation of the telegram api in similar naming schemes.

##### Bitcoin
Bitcoin is known as a "anonymous" currency. Where the coins cannot be traced to the original sender, and if tried will be met with difficulty.

In reality, coins can be traced with enough effort. There are ways to disguise the sender such as Mixers, but ultimately still put the sender at risk of being traced.

Using bitcoin as a user is easy enough. Sign up with a wallet and then deposit money like any normal bank account, finally send money to a specified address.
Users can see a transaction ID associated with the block being verified depending on the wallet's capabilities. Coinbase shows a TxID but you'd have to do quite some digging. Cashapp has no way to show TxID.

There's a small fee associated with sending money and can be expensive during high bitcoin traffic hour.