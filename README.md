# SpaceXpanse Multiverse manifesto
### To set the intentions    

>I think that the crypto industry will have to take a more focused approach, shifting from hype cycles toward building real utility.  
 Rahul Advani  - Ripple’s APAC Policy Director

**Long story short**:  
We want to ***turn the [crypto] game around*** /pun intended/ <!-- First we wanted to create a great game, now we want to change the world-->
  
By *putting the crypto technology back on track*, we are making a next-generation trustless blockchain platform, designed for rapid creation of metaverses, immersive user experience and easy development of complex decentralized applications, which we called **SpaceXpanse Multiverse**, where people can communicate, create, have fun, and which can be easily accessed by anyone from anywhere.  

## SpaceXpanse Multiverse /SpeX/ platform environment: 

### Technologies 
[**ROD blockchain**](https://github.com/SpaceXpanse/rod-core-wallet/tree/0.6.8/doc/spacexpanse)  
Open source  
*Non-profit - Foundation operated*
- Main cryptocurrency /**ROD**/, [fungible](https://github.com/SpaceXpanse/rod-core-wallet/blob/0.6.8/doc/spacexpanse/currencies.md) and [nonfungible](https://github.com/SpaceXpanse/libspex/tree/dev/nonfungible) tokens /NFTs/ - creation, storage and transaction
- Decentralized DNS aka **dDNS** /derived from Namecoin/ which can serve **.rod** and/or other domains /WIP*/
- [Digital IDs](https://github.com/SpaceXpanse/rod-core-wallet/blob/0.6.8/doc/spacexpanse/blockchain.md#names) for platform-wide trustless user identification which can even hold and transfer value in the ROD blockchain
- Secure [storage of data](https://github.com/SpaceXpanse/rod-core-wallet/blob/0.6.8/doc/spacexpanse/blockchain.md#spacexpanse-is-based-on-namecoin-) in the blockchain **itself**.
- Local data storage for DApps **outside** blockchain by using SQLite /or LMDB/ database engine 
<!-- - Decentralized Proof of Stake aka **DPoS** masternodes and peer-to-peer nodes for secure data storage **outside** blockchain by using SQLite /or other/ database engine /TBD/ -->
- [Atomic trading](https://github.com/SpaceXpanse/rod-core-wallet/blob/0.6.8/doc/spacexpanse/trading.md) to exchange in-game assets (fungible game currencies as well as non-fungible items) in a trustless manner.   
- [Human mining](https://github.com/SpaceXpanse/rod-core-wallet/blob/0.6.8/doc/spacexpanse/games.md) aka **Play To Earn** model which allows parts of the mined block rewards to be "placed" inside an application, game or other, where users can pick/win them up and bank them to their on-chain address. /WIP/

[**ROD framework**](https://github.com/SpaceXpanse/rod-framework) - a modified version of an open-source, censorship-resistant [**Nostr**](https://github.com/SpaceXpanse/nostr) protocol that aims to provide a more decentralized, privacy-centered and user-empowered alternative to traditional centralized ways to store and retrieve huge amounts of data. /WIP/  
Open source  
*Non-profit - Foundation operated*  
Implementation follows [a set of rules](https://github.com/SpaceXpanse/nips) by using:
- [ROD relay:](https://github.com/SpaceXpanse/rod-framework) Anyone can run a relay /possibly after locking some amount of ROD in a wallet - TBD/, and they are responsible for storing the data by using one or more PostgreSQL instances, for example, and then forwarding it to other relays eventually. They can set them public or private, collect a fee for using it, etc.
- [ROD client](https://github.com/SpaceXpanse/rod-framework): Users run clients on their own computers to connect to these relays to send and receive data.  

Both can use ROD blockchain's storage capabilities to transfer data e.g. relay domain addresses, user presence between them.

<!--
[**SpeXQL**](https://github.com/SpaceXpanse/SpeXQL) -  Decentralized database management system using ROD blockchain as medium for data transfer, interconnection and operations /Deferred/  
Open source  
*Non-profit - Foundation operated*  
- Implemented using both DPoS masternodes as Block Producers and peer-to-peer data storage nodes as Data Miners, which can store platform's data and files /public and private/ -->
  
[**Side Channels**](https://github.com/SpaceXpanse/libspex/tree/dev/sidechannel) 
Open source   
*Non-profit - Foundation operated*  
- Programable trustless interconnection **inside** the blockchain which allows two or more parties to interact through temporarily made [sidechains](https://www.coindesk.com/learn/an-introduction-to-sidechains/) in a very scalable, off-chain and almost real-time fashion.

### Development

[**SpeX Library**](https://github.com/SpaceXpanse/libspex)      
Open source  
*Non-profit - Foundation operated*  
- Programable trustless interconnection **between** the blockchain and third-party applications to help developers have useful environment for effortless development of DApps in the platform  

[**SpeXID**](https://github.com/SpaceXpanse/SpeXID) - Digital Identification application for SpaceXpanse Multiverse platform /WIP/    
Open source  
*Non-profit - Foundation operated*  
- An application built on top of the ROD blockchain, that turns each reserved name into a secure digital identity similar to [NameID](https://nameid.org)  

<!-- **Democrit** - Atomic trading  
Open source   
*Non-profit - Foundation operated*  
- A protocol and system for executing atomic trades on the **SpaceXpanse Multiverse** platform. This allows players to trade their game assets for the main cryptocurrency /**ROD**/ and/or tokens in a fully trustless manner.
-->

[**RODPay** Server](https://github.com/SpaceXpanse/RODPay) - a free and open-source payment processor which allows you to accept payments without fees or intermediaries. /WIP/   
Open source    
*Non-profit - Foundation operated*
- Direct, peer-to-peer payments
- No additional transaction fees /other than the network fee/
- No fees, middleman or KYC
- Non-custodial /complete control over the private key by using a remote wallet/
- Enhanced privacy & security
- Self-hosted
- SegWit support
- Share your instance with friends /multi-tenant/
- Invoice management and Payment requests
- Apps: **Marketplace** for your digital IDs, .rod domains, etc.; **Crowdfunding** for supporting your projects; Buttons for **Donation** receiving

[**SpaceXpanse DappEngine**](https://github.com/SpaceXpanse/DappEngine) - A versatile tool for creating 2D and simple 3D games and other dapps with ease /WIP/    
Open source  
*Non-profit - Foundation operated*

- In DappEngine, everything on the screen is an object. /WIP/
- It uses events to define the logic of your game. /WIP/
- It allows you to use variables to store and manipulate data during gameplay. /WIP/
- It provides a powerful feature called "Events Function" or simply Function. /WIP/
- It includes a variety of pre-made objects such as buttons, switches, sliders, and more. /WIP/
- Its features are provided through extensions, allowing you to embed only the features you need. /WIP/
- It's a cross-platform development software. You will be able to build games and other apps for mobile, desktop, and the web. /WIP/
- It's an open-source, no-code game development software licensed under the MIT license.  
  
[**SpaceXpanse Metaverse Simulator**](https://github.com/SpaceXpanse/Metaverse) - A playground for testing different environments, tools and objects in the platform /WIP/    
Open source  
*Non-profit - Foundation operated*

- Real-time realistic solar system with major celestial bodies, terrains and environment
- Gravitational and other forces, affecting all objects accordingly /physics/
- Fast rendering with realistic level of detail /TBD/
- Node-based programming logic /TBD/
- Scenario programing through Lua - lightweight, embeddable programming language designed for scripting and extensibility
- Python support for modeling of mathematical and other scientific inquiries /TBD/
- Support for Universal Scene Description /USD/ for collaboratively building 3D sceneries, intended for large-scale production. /TBC/ 
- Easy creation and editing of new solar systems, planets and satellites, vehicles and other multi-part and multi-seated usable objects
- Simplistic interconnection with any other elements of the platform environment through dedicated API

### Community

[**Metalog**](https://github.com/SpaceXpanse/Metalog) - Decentarized Social Network /WIP/   
Open source  
*Non-profit - Foundation operated*
- Full-blown platform-wide social network in the blockchain, accessible within every platform's metaverse and/or DApp, using **Nostr** protocol to store user's private data and **ROD bockchain** for user's public data.

**SpeXDAO** - Decentralized Autonomous Organisation /Deferred/   
Open source    
*Non-profit - Foundation operated*
- Full-blown platform-wide application in the blockchain to serve as crowdfunding hub for user's projects within the platform and more

### Entertainment  

[**SpaceXpanse: Battleships**](https://github.com/SpaceXpanse/Battleships) - The classic game of Battleship, but with a twist /WIP/  
Open-source  
Non-profit - Foundation operated  
Simple multiplayer online game in the ROD blockchain  

- Developed on top of **libspex**'s headless Ships game with the help from various development tools.
- Made with **Unity**
- Simplistic gameplay: Two players can choose to compete with each other's tactical combat, strategic skills and shear luck for a prize that they agreed upon in the beginning
- Ability to compare players' scores through Leaderboard
- Owning NFTs to straighten spaceship's attack and defense capabilities /TBA/
- In-game communication in real time through **Metalog** /TBD/

**SpaceXpanse: Wanderers** - A space exploration game in its own metaverse /TBD/    
Closed-source  
*For-profit - Legal entity operated*  
Real-time Massive Multiplayer Open World Sandbox game with realistic look, physics and economics  
- Developed on top of **SpaceXpanse Metaverse Simulator** with the help from various development tools /TBA/. <!-- - Partly closed source /for the game engine and game logic/ -->
- Made with **Unreal Engine 5** <!-- and Vulcan -->
- Sophisticated gameplay: Player versus Environment aka PvE /possible addition of PvP/, massive near-real economy, tactical combat and strategic skills development
- In-game communication in real time /through **Metalog**/
- Creation and customization of avatars <!-- - Voice-activated commands -->
- NFTs for ownership of land, objects and goods
- <!-- Decentralized --> Artificial intelligence <!-- and machine learning -->for automation of the gameplay <!-- : NPCs, mining, defence, navigation and communication --> /TBD/
- VR gaming <!-- for mobile phones. XR too -->
<!-- - A possibility for real-time monitoring and customization of story arcs /scenario injection/ -->
<!-- - Enable users to fund projects like custom-made objects through **MetaDAO** -->
<!-- 
***The Voyagers Chapter***  
Where users can explore the solar system and have access to limited missions /sandbox for the next chapter/ 

***The Prospectors Chapter***  
Where users can also claim land, dig its resources, build multi-part objects and do limited trade with them /sandbox for the next chapter/

***The Merchants Chapter***  
Where users can also buy, lend and sell what they want in near-real economy 

***Infinity Chapter***
Warp drive invention to explore Milky Way galaxy and beyond. 
 -->
----
*Further sophistication of the subject is covered in the [Whitepaper](https://github.com/SpaceXpanse/Whitepaper/wiki)*.  
*To get a notion of the time table and completeness of these intentions, visit [Roadmap](https://github.com/SpaceXpanse/Roadmap)*.

---- 
#### Legend
WIP - Work in progress  
TBA - To be announced  
TBC - To be confirmed  
TBD - To be determined  
