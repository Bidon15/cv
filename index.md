# Anatolii Osetsymskyi

_Rust/C++/GO Software and Blockchain Developer, Live in Amsterdam, Netherland. Resident of Ukraine 🇺🇦_

[Email](mailto:xgreenx9999@gmail.com) / [LinkedIn](https://www.linkedin.com/in/aostesymskyi/) / [GitHub](https://github.com/xgreenx) / [Telegram](https://t.me/xgreenx99) / +380663944720

## 🔧 Development preferences 

- Main languages:
  - Rust - the language that I prefer to work with. I enjoy its features, proc macros, and memory management.
  - C/C++ - my first language from the university. I like its low-level stuff.
  - Golang - goroutines are a fantastic feature and a perfect fit for writing asynchronous code.
- Secondary languages:
  - Javescript/Nodejs - every project that I worked on somehow required the usage of JS.
  - Swift/Objective-C - in my free time, I like to develop some applications on my smartphone.
  - C#/Java - studied in the university and after interacting with it on different works.
  - Haxe - it is an unusual language, but I used it for around two years together with C++.
  - Python - in the university, I played with machine learning, and I have basic knowledge of that language.
- OS:
  - Mac OS - last 2 years I'm using that system as main.
  - Linux - it was the primary system for development before Mac OS. I worked with Ubuntu image and tried Debian and other distributives in most cases.
  - Windows - used that system for development at the beginning of my career. But honestly, it doesn't fit for development=)
	

## 💼 Work experience

**Rust Core Blockchain Developer** [Supercolony](https://supercolony.net) _(April 2021 - Present)_

The work is related to evolving of the ecosystem and WASM smart contract development. Except for that, 
there was several project of portfolio companies related to ink!, substrate development.
- Successfully ported two big projects from Solidity to ink!(30+ contracts) that increased the coverage of audience.
- Designed and implemented [OpenBrush](https://github.com/Supercolony-net/openbrush-contracts) as a first library(analog of OpenZeppelin) to ease out WASM smart contract development experience in the dotsama community.
- Implemented functionality for upgradeable contracts on all execution layers.
- Designed(traits - soon link to the issue, [event](https://github.com/paritytech/ink/pull/1243) refactoring) and implemented([storage](https://github.com/paritytech/ink/issues/1134), [dispatching](https://github.com/paritytech/ink/pull/1017)) major features in the ink! to improve the language syntax and simplify the development.
- Designed the architecture of substrate-based blockchain with inner yield protocols.
- Decreased the size of smart contracts(10-15%) to improve on-chain performance.
- Designed and implemented standards of [Fungible](https://github.com/w3f/PSPs/blob/master/PSPs/psp-22.md), [Non-Fungible](https://github.com/w3f/PSPs/blob/master/PSPs/psp-34.md), and [Multi tokens](https://github.com/w3f/PSPs/blob/master/PSPs/drafts/psp-35.md) to unify the interface for the WASM smart contract ecosystem.
- Optimized(x25) the Graph indexer for PancakeSwap to process transactions with the speed of the binance smart chain.

During the work, I interviewed candidates.

**GO/C++/Rust Core Blockchain Developer** [ProximaX](https://www.proximax.io) _(April 2020 - April 2021)_

The main idea of the project is decentralized storage(DFMS written on Golang) built on top of 
the blockchain(C++) with an execution layer for smart contracts(WASM Rust/TS Assemblyscript).
- Design(for the blockchain and DFMS) a new, more secure version of the storage with an improved flow for users and storage providers.
- Implemented main plugins(analogs of Cosmos Modules but on C++) of a new business logic on the blockchain.
- Refactored the logic of the Merkel tree calculation and optimized(x2) the work of the unconfirmed cache.
- Refactored the [Golang SDK](https://github.com/proximax-storage/go-xpx-chain-sdk) to be compatible with a new blockchain version.
- Fully rework the execution level of the DFMS:
  - Implemented a new system of events to parallelize the execution and fix previous bugs related to conflicting executions.
  - Changed the work with storage to lock only data cells related to execution instead of the whole storage.
  - Added support of new host functions and integrated them into VM to increase the functionality.
  - Designed and implemented the consensus of executors for non-deterministic operations like HTTP requests etc.
- Implemented simple [TS Assemblyscript](https://github.com/proximax-storage/ts-xpx-supercontract-sdk) to write smart contracts with TypeSccript and compile them into WASM to run on executors.
- Refactored IPFS of the file system to be compatible with blockchain structure.
- Debugging and fixing bugs on the blockchain side related to an inconsistent state, corrupted pointers, incorrect state reverts, vulnerabilities related to DDoS, and invalid transaction propagation.

**C++/GO Blockchain Developer** [482.solutions](https://482.solutions) _(August 2018 - April 2020)_

It was a company where I started work with blockchain.
The main project was the customization and updating of the NEM blockchain, 
adding new features, new plugins, performance testing, and optimizations. 
Side projects were related to the integration of the blockchain with IoT.
- Added metrics into the code and created a framework for performance testing of the blockchain. 
  Based on the results of the testing:
  - Optimized the processing of common transactions(x3) and custom transactions(x1.5).
  - Found and fixed several bugs with race conditions and reported them to the NEM team.
  - Found vulnerability with DDoS protection against invalid transactions that we fixed by changing the token economic model.
  - Those metrics and that framework were used during network upgrades to find and fix regressions.
- Designed and developed the first version of DFMS and integrated it with the blockchain. Integration includes:
  - Implement new plugins on the blockchain to support storage manipulations and charge tokens for storage usage. 
  - Actualization and refactoring of the [Golang SDK](https://github.com/proximax-storage/go-xpx-chain-sdk) for interactions with blockchain.
  - Integration of new SDK and business logic into DFMS and CLI.
  - All changes include the unit and e2e testing.
- Developed a C++ SDK to interact with NEM/ProximaX blockchain from IoT devices.
- Developed several examples of how IoT devices can interact with blockchain to show 
  different use cases where blockchain can be integrated into real life.

The work also included CI, adding and gathering of logs from different users and their analysis via kibana and elasticsearch.

**Junior Haxe/C++ Developer** [The Product Engine](https://www.productengine.com) _(October 2016 - August 2018)_

Most tasks were support and development of a new UI(Haxe) for different DVRs.
But also ware tasks related to performance, rendering, memory leaks, debugging and implementing a new API on the backend side.
- Refactored OneLineGuide(a separate screen to easily navigate TV shows)
  to be compatible with the new UI. Changed the layout logic to work faster and send fewer requests.
- Reimplemented the logic of the backend for Filtered Guide(a separate screen allows filtering content) to not crash with searches with a lot of content.
- Removed a lot of memory leaks during image loading and caching and decreased the application's memory consumption two times.
- Fixed different bugs related to text rendering in OpenFL on different platforms.
- Found the root cause of several strange issues that were faced by some users sometimes via objdumping and debugging assembler code.

During the work, I used a lot of Splunk to analyze the performance and stability of the screen developed by the team.

**Junior C++/QT Developer** [ODISW](http://sprut-ow.net) _(January 2016 - June 2016)_
Development of street lighting management project cities for several cities in Ukraine: Kirovograd, Mariupol, Mykolaiv, Theodosius, etc.
- Stabilization the project to not crash.
- Developed a new type of the user's terminal from scratch to remotely work with a more advanced electric control system..

**Junior Swift/Objective-C** Freelance _(Jul 2015 - January 2016)_
Developing an application for managing surveillance cameras from IOS(iPhone or iPad) via FFmpeg.
POC of the client application and the MVP were developed quickly.
After the designer created mockups, and I applied them to the project.
The project is not live in the App Store due to a lack of funding and changing customer's plans.

## 📖  Education
**Diploma Master's degree of the Applied Mathematics.** in Odessa National University I.I.Mechnikov<br>
[Mechnikov University](http://onu.edu.ua/en/) - Odessa, Ukraine _(2018 - 2020)_

**Diploma Bachelor of the Applied Mathematics** in Odessa National University I.I.Mechnikov<br>
[Mechnikov University](http://onu.edu.ua/en/) - Odessa, Ukraine _(2014 - 2018)_

**[Data Science: Deep Learning in Python](https://www.udemy.com/course/data-science-deep-learning-in-python/)** on Udemy<br>
[Course Udemy](https://www.udemy.com) by Lazy Programmer Inc. _(2018)_

## 🏆 Accomplishments

**Desktop Sharing Application** _(2019)_ <br>
Developed an analog of TeamViewer for local usage called [Desktop Sharing](https://github.com/xgreenx/desktop-sharing) 
via go-libp2p, c-go and FFmpeg.

**24th place on ½ ACM-ICPC programming olympiad** _(2017)_ <br>
My team [ONU_Luckomotive](https://icpc.global/regionals/finder/SEERC-2017/standings).

**Solved many programming olympiad problems** _(2016-2017)_ <br>
To improve my skill in olympiad programming solved many problems on different online platforms for training:
- [Timus](http://acm.timus.ru/author.aspx?id=189179)
- [Codeforces](http://codeforces.com/profile/xgreenx9999)
- [E-olymp](https://www.e-olymp.com/ru/users/XGreenX99)

## 👤 About
I have an inquisitive mind and enjoy solving different problems. I like to come up with a solution to the problem,
implement it and watch how well it works :)

In my free time, I like to spend time with friends playing board games 🎲 and computer games 👾.
Like everything that is related to mathematics :)

I like to leave "=)", ":)" or "=D" everywhere =D