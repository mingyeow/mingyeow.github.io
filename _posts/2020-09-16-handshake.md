---
layout: post
title:	Handshake - A Namespace For The Decentralized Web
date:	2020-09-14
author:	Ming Ng, Cassandra Shi, Andrew Lee
description: The first post on this website.
subtitle: The core of the Handshake experiment isn’t tech or cryptography - It’s names
---

Names are fundamental to human existence and how we relate to everything in the world. At the heart of all interactions lies the ability for all the parties to match names to the respective entities they stand for. Names are so integral to the human experience that a strong argument can be made that if _something doesn't have a name, it does not exist._

Correspondingly, names on the internet are critical to our online existence. Users, apps, or machines locate a resource on the internet via its name. The name needs to not only be understood by humans but also needs to be uniquely identifiable by machines amongst the billions of potential destinations. 

Given that the act of matching a name to the eventual resource is the starting point of trillions of internet transactions that happen daily,  it is no surprise that out of the three core layers of internet stack - naming (DNS), transportation (TCP/IP) and application (HTTP), naming is at the very start of the stack. 

Naming needs a single source of truth as the names within the namespaces have to be unique across the whole system. Hence, an effective naming system cannot merely be a standard or a protocol, it has to meet all the other aspects of running an internet-scale namespace - including enforcement of unique names, the management of the naming records, scaling to internet traffic, while remaining fully accessible to anyone, anywhere.

**Namespaces**

Names are the most valuable assets on the internet, but we don’t own our own names. All of the crucial namespaces belong to centralized entities who control the namespaces and take that control away from you. This is true for all significant namespaces today - the ICANN namespace, Facebook, Twitter, and Google. 

As a result, your name on the internet does not belong to you, but rather to the owners of these centralized namespaces.  With a stroke of the keyboard, they can remove anyone from existence.  If your name lives on a centralized namespace, your right to exist effectively belongs to someone else. 

Centralized namespaces also determine much more than a user's ability to exist. They also decree a user's ability to search, match, and communicate with others. They unilaterally set the framework for what protocols can be used, which use cases are permitted, and what information can flow.

The power to enforce monopolies with little consequence also makes these centralized namespaces some of the most valuable properties on the internet today. Verisign makes billions a year controlling .com with practically zero innovation, while ICANN has the power to arbitrarily raise price caps of entire TLDs with their pet cartel companies. Facebook and Twitter controls exactly how users can use their names/accounts, and can heedlessly cancel pages and remove identities for barely specified reasons. 

Everywhere we see, we are seeing the serious dangers of depending on centralized entities to exist and be found by others. The Internet is supposed to be kingless, but the ability to strike away one's existence and control exactly how the name is to be used makes the owners of these namespaces the de-facto kings/governors of the internet.

**The World Needs a Decentralized Namespace**

Of course, the ability of these centralized namespace owners to control digital existence, lockout access, and enforce monopolistic economics is the complete opposite goal of the decentralized web, which is the ability to exist, innovate, and create their own business models without the need for centralized control or systems. 

Whether it's decentralized currencies, decentralized file systems, or decentralized servers - if these decentralized entities do not live on a widely used namespace, they simply do not exist to the vast majority of users on the internet. 

_Without a decentralized namespace widely readable by humans and resolvable by machines, it is impossible for the decentralized world to be widely adopted by users_.

**Criteria for a Decentralized Naming System**

Naming systems play a crucial role in discovery, connection and identification. As one of the most fundamental and long-lasting components of the internet backbone infrastructure, the bar needs to be set very high in terms of longevity, stability, and technical scalability. 

For a decentralized naming system to become the legitimate namespace for the decentralized world, the bar is even higher. Without a centralized body in charge, the world has to trust that this naming system will exist in a stable state for a long time to come and stay relevant regardless of potential upheavals and technological progress. 

As such, this naming system's fundamental construction needs to have certain key technical, social, and governance requirements:



1. Be truly decentralized: what is the point of a decentralized naming system if it remains controlled by a small set of people?
2. Maintain a key focus as a naming system: naming systems need to be extremely focused and fast. Can you imagine the DNS system operating reliably if it was also designed for delivering 4K video?
3. Be as accessible yet trustless as possible: anyone should be able to access the namespace directly in a fully trustless manner without intensive resources
4. Compatible with the rest of the internet: allowing for seamless usage with the rest of the application, user, and technical stack 
5. Stability and upgradability at the protocol level: allowing for innovation moving forward without disrupting regular operations 

**Handshake Design**

Given these objectives, and with the general goal of the decentralized root zone and certificate authority, Handshake is the only naming system that is fundamentally suitable to be the namespace for decentralized web.

**1. Focus as a Naming System**

Let's consider the inherent complexity of an internet-scale naming system. For reference, the naming layer (DNS), unlike the other layers of the internet stack, is the only layer that is a system and not a protocol - the key difference between the two is that a protocol cannot enforce uniqueness of names, which is essential to a functioning namespace. It's also arguably by far the most complex layer with many competing technical, political, and economical demands. 

As a standalone blockchain, Handshake has room to grow all on its own and govern itself without interfering with other projects or having to compete with different priorities with other use cases (like gaming or DeFi) trying to run in parallel on the same network. In addition, there are several fundamental constraints in other blockchains - for example, Bitcoin limited OP sizes and Ethereum's notoriously hard to sync blockchain. 

If Handshake is built on another blockchain, the instability caused by these competing priorities for use cases and political interests also eliminates one of the core requirements for a decentralized naming infrastructure - which is stability. A naming infrastructure needs to be highly stable - remember - both users, hosts and developers need to be confident that the names will be around for a long time in the same format. For instance, Ethereum's sky high gas prices due to DeFi and the complex migration to ETH2 are both creating high levels of certainty around how apps will work in the future, and whether retail users will be able to have the same level of access as large ticket users.

Lastly, creating a native auction system is complicated and requires highly specific primitives, such as making coins unspendable for certain periods, and increases the complexity of the system if HNS is a non-native token.

**2. Decentralization**

The other critical consideration is decentralization. _Remember, the goal here is to achieve a truly decentralized, uncensorable namespace independent of centralized control and policies. Anything less than will be completely redundant._

Ethereum is the most decentralized smart contract platform of date, but it's still insufficient as a base layer blockchain for a truly decentralized naming system. A system based on Ethereum either would have to be strictly immutable or engineer a governance mechanism with a single or multiple signers. For example, the ENS system on Ethereum has a 7-part multisig making it either censorable and shutting it off to any future innovations or upgrades. These mechanisms either risk shutting off future innovations or don't meet the decentralized requirement.

How about sidechains? Sidechains mostly rely on the main chain's security, which makes them completely subject to the same concerns above in terms of sharing priorities with the main chain. In addition, there is currently no such thing as a decentralized side-chain on Bitcoin. Counterparty is a one-way system, Liquid requires a small federated multisig, and Rootstock is currently federated waiting on Drivechain support from Bitcoin. 

For all of PoW's issues, namely with the limited number of miners, it is built on competition which is inherently decentralized as well as clear separation of concerns between developers, users, and miners. This is in contrast to PoS which encourages stakeholders to collude and centralize, creating a largely plutocratic environment. 

As such, true naming decentralization with the ability to upgrade is likely best achieved on a standalone PoW chain with robust hash power, a strong ecosystem, and miner confidence in the value of the blockchain. 

**3. Ease of Trustless Resolution**

Compared to other naming blockchains, _the entire Handshake stack is engineered for the use case of creating a human readable, truly decentralized, fully accessible and secure namespace. _

The naming data in Handshake is stored in a novel data structure called an Urkel Tree,  which was designed specifically for this purpose. The proofs are small and verify quickly, allowing name resolution to happen with very little computation. 

Secondly, a highly unique application called HNSD written in C only handles the DNS functions of Handshake (avoiding any primitives related to currency). It is designed to be as fast as possible and as lightweight as possible. Written in C, it can be compiled on every computer system in use today. HNSD verifies compact proofs, which cryptographically ensure that a DNS record is on the Handshake blockchain, and in the chain with the most accumulated proof-of-work. 

The light resolver means anyone can use Handshake with minimal effort. The efficiency provided by the compact Urkel proofs means that Handshake resolution can be executed on the most minimal of devices.

As a result, Handshake is the only naming system that allows anyone with any level of resources to access the namespace without the need for any centralized components, and without any level of security tradeoffs. Depending on their preferences, a user or application can resolve names by running a full node, a HNSD client, or a third-party resolver. In many ways, this spectrum of accessibility is the gold standard for a trustless naming resolution system.

**4. Compatible with the Rest of the Internet**

HNS works with the entire DNS stack in all the key ways - technical, resolution and for new systems, without being hampered by the political, economic and technical burdens of DNS

Handshake doesn't replace the ICANN root zone, it extends it. When queried for a name, the Handshake resolver checks the blockchain for the TLD first. If it does not find it there, it then "falls back" to ICANN's DNS system. A user running Handshake can browse the entire internet just like they always have, but now they can also resolve names rooted in the blockchain. 

After the root zone, there is no difference between DNS resolution on Handshake or the legacy system. Resolvers follow the chain of domains and sub-domains indicated by a URL and connect with authoritative nameservers around the world running the same software they always have.

**5. Stability and Upgradability at the Protocol Level**

Handshake allows up to 512 bytes of anything to be inserted in the Urkel tree for a name. Currently, all Handshake software is configured to only allow read/write of format-compliant DNS records, but it is trivial to write software that uses the data available for other purposes.

In addition, PoW is the most robust mechanism we know of today to provide infrastructural level stability while having a clear upgrade path. 

As for governance, the most interesting thing philosophically about HNS is the experimentation of a kingless construct. There is no leader, no foundation, and no core team post launch. Handshake follows the same upgrade path as Bitcoin via soft forking and offchain social coordination, which is proven to be the most resilient mechanism for governance. 

Alternative approaches like PoS governance are still in early stages and haven’t withstood the test of time. The ENS approach is even more vulnerable, where a group of multisig key holders, no matter how reputable, will control the governance and upgrade of the backbone infrastructure of the decentralized web.

Handshake and Bitcoin are two truly decentralized projects without kings, and the crypto space should be about exploring alternative coordination mechanisms. We will cover this topic in a later essay.

**Handshake: Extending the Internet**

The idea of centralized systems controlling names is fundamentally incompatible with the decentralized web, which needs to be independent of any centralized ingredients.  

Without a widely resolvable and recognized naming system, the decentralized web, and everything on it (decentralized servers, decentralized filespaces) will be invisible, and therefore, does not exist to wide swathes of the mainstream world. 

HNS is the only namespace designed to withstand the length of time, infinitely extensible use cases and maintains the complete spectrum of convenience/decentralization tradeoffs. 

It will of course take a while to get to the widespread adoption needed, but that curve of legitimacy is not dissimilar to the curves of validation that Bitcoin had to take before being recognized as a legitimate store of value and one of the prime contenders for value alongside gold and USD.

By making the decentralized web just as accessible as the centralized ones, HNS looks to extend the internet beyond its current borders.  If you are interested to be part of this movement, we strongly encourage you to become part of the ecosystem - join the groups, get some HNS, secure a name. 

Most of all, participate in the community by providing code, ideas, or just good vibes. It’s early days yet for Handshake, the decentralized web, and most of all, what it means for all of us to exist, collaborate and coordinate on the Internet. 

Would be great to have you along for the ride.