# The SpaceXpanse Multiverse /SpeX/ platform    
### The metaverse of the future  
***A comprehensive  manifesto of the intentions for the next few years***  

>I think that the crypto industry will have to take a more focused approach, shifting from hype cycles toward building real utility.  
 Rahul Advani  - Ripple’s APAC Policy Director

**Long story short**:  
We want to ***turn the [crypto] game around*** /pun intended/ <!-- First we wanted to create a great game, now we want to change the world-->
  
By *putting the crypto technology back on track*, we are making a next-generation trustless GameFi platform, powered by blockchain technology and artificial intelligence, and designed for rapid creation of metaverses, immersive user experience and easy development of complex decentralized applications, which we called **SpaceXpanse Multiverse**, where people can communicate, create, have fun, and which can be easily accessed by anyone from anywhere.  

## The platform environment: 

### Technologies 
#### [**ROD blockchain**](https://github.com/SpaceXpanse/rod-core-wallet/tree/0.6.8/doc/spacexpanse)  
Open source  
[*Non-profit - Foundation operated*](https://opencollective.com/spacexpanse)  
- Main cryptocurrency /**ROD**/, [fungible](https://github.com/SpaceXpanse/rod-core-wallet/blob/0.6.8/doc/spacexpanse/currencies.md) and [nonfungible](https://github.com/SpaceXpanse/libspex/tree/dev/nonfungible) tokens /NFTs/ - creation, storage and transaction
- Decentralized DNS aka **dDNS** /derived from Namecoin/, which can serve **.rod** and/or other domains /WIP*/
- [Digital IDs](https://github.com/SpaceXpanse/rod-core-wallet/blob/0.6.8/doc/spacexpanse/blockchain.md#names) for platform-wide trustless user identification, which can even hold and transfer value in the ROD blockchain
- Secure [storage of data](https://github.com/SpaceXpanse/rod-core-wallet/blob/0.6.8/doc/spacexpanse/blockchain.md#spacexpanse-is-based-on-namecoin-) in the blockchain **itself**.
- Local data storage for DApps **outside** blockchain by using [SQLite](https://github.com/SpaceXpanse/Documentation/wiki/Hello-World-with-SQLite) /or LMDB/ database engine 
<!-- - Decentralized Proof of Stake aka **DPoS** masternodes and peer-to-peer nodes for secure data storage **outside** blockchain by using SQLite /or other/ database engine /TBD/ -->
- [Atomic trading](https://github.com/SpaceXpanse/democrit-marketplace) to exchange in-game assets (fungible game currencies as well as non-fungible items) in a trustless manner.   
- [Human mining](https://github.com/SpaceXpanse/rod-core-wallet/blob/0.6.8/doc/spacexpanse/games.md) aka **Play To Earn** model, which allows parts of the mined block rewards to be "placed" inside an application, game or other, where users can pick/win them up and bank them to their on-chain address. /WIP/
<!--
[**SpeXQL**](https://github.com/SpaceXpanse/SpeXQL) -  Decentralized database management system using ROD blockchain as medium for data transfer, interconnection and operations /Deferred/  
Open source  
*Non-profit - Foundation operated*  
- Implemented using both DPoS masternodes as Block Producers and peer-to-peer data storage nodes as Data Miners, which can store platform's data and files /public and private/ -->
  
#### [**Side Channels**](https://github.com/SpaceXpanse/libspex/tree/dev/sidechannel) 
Open source   
[*Non-profit - Foundation operated*](https://opencollective.com/spacexpanse)    
- Programable trustless interconnection **inside** the blockchain which allows two or more parties to interact through temporarily made [sidechains](https://www.coindesk.com/learn/an-introduction-to-sidechains/) in a very scalable, off-chain and almost real-time fashion.

### Development

#### [**SpeX Library**](https://github.com/SpaceXpanse/libspex)      
Open source  
[*Non-profit - Foundation operated*](https://opencollective.com/spacexpanse)   
- Programable trustless interconnection **between** the blockchain and third-party applications to help developers have useful environment for effortless development of DApps in the platform  

#### [**SpeXID**](https://github.com/SpaceXpanse/SpeXID) - Digital Identification application for SpaceXpanse Multiverse platform /WIP/    
Open source  
[*Non-profit - Foundation operated*](https://opencollective.com/spacexpanse)   
- An application built on top of the ROD blockchain, that turns each reserved name into a secure digital identity similar to [NameID](https://nameid.org)

#### [**Democrit**](https://github.com/SpaceXpanse/democrit-marketplace) - Trustless Marketplace Framework employing the features of ROD blockchain /WIP/   
Open source   
[*Non-profit - Foundation operated*](https://opencollective.com/spacexpanse)   
- A protocol and system for executing trustless atomic trades on the **SpaceXpanse Multiverse** platform. This allows developers to integrate trading of their DApp/game assets for the main cryptocurrency /**ROD**/ and/or tokens in a fully trustless manner.

#### [**RODPay** server](https://github.com/SpaceXpanse/RODPay) - a free and open-source payment processor which allows you to accept payments without fees or intermediaries. /WIP/   
Open source    
[*Non-profit - Foundation operated*](https://opencollective.com/spacexpanse)   
- Direct, peer-to-peer payments
- No additional transaction fees /other than the network fee/
- No fees, middleman or KYC
- Non-custodial /complete control over the private key by using a remote wallet/
- Enhanced privacy & security
- Self-hosted
- SegWit support
- Share your instance with friends /multi-tenant/
- Invoice management and Payment requests
- Included apps:
  - **Marketplace** for your digital IDs, .rod domains, etc.;
  - **Crowdfunding** for supporting your projects;
  - Buttons for **Donation** receiving

#### [**ROD-to-Nostr framework**](https://github.com/SpaceXpanse/rod-to-nostr-framework) - a modified version of an open-source, censorship-resistant [**Nostr**](https://github.com/SpaceXpanse/nostr) protocol that aims to provide a more decentralized, privacy-centered and user-empowered alternative to traditional centralized ways to store and retrieve huge amounts of data. /WIP/  
Open source  
[*Non-profit - Foundation operated*](https://opencollective.com/spacexpanse)    
Implementation follows [a set of rules](https://github.com/SpaceXpanse/nips) by using:
- [Data relay](https://github.com/SpaceXpanse/rod-to-nostr-framework?tab=readme-ov-file#relay)
  - Anyone can run a relay, and they are responsible for storing the data and then forwarding it to other relays eventually. They can also set them public or private, collect a fee for using it, run one or more database instances for redundancy, etc.
  - Their addresses can be served by the ROD blockchain's **dDNS** feature and sit behind a **.rod** domain for convenience and better platform integrity. 
  - Also, by applying some custom logic through the [libspex](https://github.com/SpaceXpanse/libspex) library and by **staking** or paying some RODs through the remote wallet of a [**RODPay** server](https://github.com/SpaceXpanse/RODPay) for example, one can benefit from having a trusted account, special access, yield farming, data mining, etc. /TBD/
- [Data client](https://github.com/SpaceXpanse/rod-to-nostr-framework?tab=readme-ov-file#client)
  - Users can run clients on their own computers, or from the web, to connect to these relays to send and receive data.
- [Data vending machines](https://github.com/SpaceXpanse/data-vending-machines)
  - Nostr protocol can act as a marketplace for data processing, where users request jobs to be processed in certain ways (e.g., “speech-to-text”, “summarization”, etc.), but they don’t necessarily care about “who” processes the data.

All of them can use ROD blockchain's capabilities to transfer data, e.g. relay domain addresses, user presence between them.

#### [**SpaceXpanse DappEngine**](https://github.com/SpaceXpanse/DappEngine) - A versatile tool for creating 2D and simple 3D games and other dapps with ease /WIP/    
Open source  
[*Non-profit - Foundation operated*](https://opencollective.com/spacexpanse)   

- In DappEngine, everything on the screen is an object. /WIP/
- It uses events to define the logic of your game. /WIP/
- It allows you to use variables to store and manipulate data during gameplay. /WIP/
- It provides a powerful feature called "Events Function" or simply Function. /WIP/
- It includes a variety of pre-made objects such as buttons, switches, sliders, and more. /WIP/
- Its features are provided through extensions, allowing you to embed only the features you need. /WIP/
- It's a cross-platform development software. You will be able to build games and other apps for mobile, desktop, and the web. /WIP/
- It's an open-source, no-code game development software licensed under the MIT license.  
  
#### [**SpaceXpanse Metaverse Simulator**](https://github.com/SpaceXpanse/Metaverse) - A playground for testing different environments, tools and objects in the platform /WIP/    
Open source  
[*Non-profit - Foundation operated*](https://opencollective.com/spacexpanse)   

- Real-time realistic solar system with major celestial bodies, terrains and environment
- Gravitational and other forces, affecting all objects accordingly /physics/
- Fast rendering with realistic level of detail /TBD/
- Node-based programming logic /TBD/
- Scenario programming through Lua - lightweight, embeddable programming language designed for scripting and extensibility
- Python support for modeling of mathematical and other scientific inquiries /TBD/
- Support for Universal Scene Description /USD/ for collaboratively building 3D sceneries, intended for large-scale production. /TBC/ 
- Easy creation and editing of new solar systems, planets and satellites, vehicles and other multi-part and multi-seated usable objects
- Seamless integration with ROD blockchain by using [**libspex**](https://github.com/SpaceXpanse/libspex) library and Nostr for enabling features like secure logins, messaging, easy payments, creation and management of NFTs and tokens, etc.
- Simplistic interconnection with any other elements of the platform environment through dedicated API

#### **Integration tools for interconnecting to other blockchains** /TBD/  
Open source   
[*Non-profit - Foundation operated*](https://opencollective.com/spacexpanse)   
- It will provide the tools to run an interface layer based on another blockchain, but which exposes a [ROD core wallet](https://github.com/SpaceXpanse/rod-core-wallet/tree/0.6.8/doc/spacexpanse) RPC interface so that logics built with [libspex](https://github.com/SpaceXpanse/libspex) can run out-of-the-box on that other blockchain.

### Community

#### [**Metalog**](https://github.com/SpaceXpanse/Metalog) - Decentralized Social Network /WIP/   
Open source  
[*Non-profit - Foundation operated*](https://opencollective.com/spacexpanse)   
- Full-blown platform-wide social network in the blockchain, accessible within every platform's metaverse and/or DApp, using **Nostr** protocol to store user's private data and **ROD blockchain** for user's public data.

**SpeXDAO** - Decentralized Autonomous Organization /Deferred/   
Open source    
*Non-profit - Foundation operated*
- Full-blown platform-wide application in the blockchain to serve as crowdfunding hub for user's projects within the platform and more

#### [**Startup Hub**](https://github.com/SpaceXpanse/Startups) -A comprehensive ecosystem around our SpaceXpanse Multiverse platform to support new and upcoming projects /WIP/   
Open source    
[*Non-profit - Foundation operated*](https://opencollective.com/spacexpanse)   
- It will not only provide news and information through [a dedicated news website](https://www.cryptospace.today/p/about-this-website.html), but will also include a dedicated section for new projects, where you can showcase your project and connect with potential investors and advisors.
- It will provide educational resources and tools to help you create and navigate the complex world of cryptocurrencies.
- It will also provide a forum for discussion, networking, and collaboration. Whether you're a gamer, developer, creator, scientist, investor, visionary, or just a crypto enthusiast, our community will be the perfect place to connect with others who share the same interests.
- And [Hackathons](https://github.com/SpaceXpanse/Hackathons) will play a significant role in the SpaceXpanse Multiverse startup ecosystem by fostering innovation, collaboration, and problem-solving.

#### [**D.A.R.M.A.**](https://www.spacexpanse.org) a.k.a Decentralized Artificial Responsive and Multipurpose Automate  
Open source   
[*Non-profit - Foundation operated*](https://opencollective.com/spacexpanse)   
- It started as an OpenAI based artificial intelligence chatbot designed to assist users becoming familiar with the platform features, programming and troubleshooting, and working across different platforms like the web, Telegram, and Discord.
- But as the platform develops further, it will become more and more integrated into the platform's features to add functionality and make it easier to work with.

### Entertainment  

#### [**SpaceXpanse: Metaverse**](https://github.com/SpaceXpanse/Metaverse) - An actual, unstoppable, and immutable metaverse, aka autonomous world, dedicated to exploring SpaceXpanse Multiverse features using the SpaceXpanse Metaverse Simulator. /WIP/    
Open source  
[*Non-profit - Foundation operated*](https://opencollective.com/spacexpanse)   

- Real-time realistic solar system with major celestial bodies, terrains and environment
- Gravitational and other forces, affecting all objects accordingly /physics/
- Fast rendering with near realistic level of detail /TBD/
- Scenario programming through Lua - lightweight, embeddable programming language designed for scripting and extensibility
- Easy creation and editing of multi-part and multi-seated usable objects
- Seamless integration with ROD blockchain by using [**libspex**](https://github.com/SpaceXpanse/libspex) library and Nostr for enabling features like secure logins, messaging, easy payments, creation and management of NFTs and tokens, etc.
- Simplistic interconnection with any other elements of the platform environment through dedicated API

#### [**SpaceXpanse: Battleships**](https://github.com/SpaceXpanse/Battleships) - The classic game of Battleship, but with a twist /WIP/  
Open-source  
[*Non-profit - Foundation operated*](https://opencollective.com/spacexpanse)   
Simple multiplayer online game in the ROD blockchain  

- Developed on top of **libspex**'s headless Ships game with the help from various development tools.
- Made with **Unity**
- Simplistic gameplay: Two players can choose to compete with each other's tactical combat, strategic skills and shear luck for a prize that they agreed upon in the beginning
- Ability to compare players' scores through Leaderboard
- Owning NFTs to straighten spaceship's attack and defense capabilities /TBA/
- In-game communication in real time through **Metalog** /TBD/

#### **SpaceXpanse: Wanderers** - A space exploration game in its own metaverse /TBD/    
Closed-source  
*For-profit - Legal entity operated*  
Real-time Massive Multiplayer Open World Sandbox game with realistic look, physics and economics  
- Developed on top of **SpaceXpanse Metaverse Simulator** with the help from various development tools /TBA/. <!-- - Partly closed source /for the game engine and game logic/ -->
- Made with **Unreal Engine 5** <!-- and Vulcan -->
- Sophisticated gameplay: Player versus Environment, aka PvE /possible addition of PvP/, massive near-real economy, tactical combat and strategic skills development
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
*Even more sophistication of the subject and technical data will covered in the upcoming [Yellowpaper](https://github.com/#)*.  
*To get a notion of the time table and completeness of these intentions, visit [Roadmap](https://github.com/SpaceXpanse/Roadmap)*.

---- 
#### Legend
WIP - Work in progress  
TBA - To be announced  
TBC - To be confirmed  
TBD - To be determined  
