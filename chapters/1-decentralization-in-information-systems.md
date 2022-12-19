# 1 Decentralization in information systems

Сentralized systems with their top-down management models have a number of disadvantages  For example, any centralized 
social network such as Facebook can censor all actions of its users and block their accounts if the actions turn out 
to be “illegitimate”. Surely, the decision on the legitimacy of these actions are solely made by the governing party.

The non-transparency of processes in such systems leaves little opportunity for consumers to prove the violation of 
their sensitive data privacy. In financial systems, this non-transparency leads to inability to verify whether a user’s 
final balance matches with the completed transactions.

Such a situation (namely, such features of the traditional architecture) allows the system owner to implement any 
modifications at his own discretion (in particular, with backdating). Obviously, decision-making is fully subjective 
in such systems.

## 1.1 What is decentralization?
The process of *decentralization* is opposite to the process of centralization. It implies that the functions of a 
particular system (storage, computation, decision-making, etc.) are maintained with the responsibility being 
distributed between the system participants. This concept is applied not only in the scope of information technologies. 
It has already been used in such areas of public life as politics, management, jurisprudence, economics, etc.

In the data transmission theory, decentralization is understood as creating conditions under which the need for a 
central server is eliminated and network participants have equal rights. The striking example of decentralization is the 
Internet: in this global network, routers operate independently of one another. In such conditions, the breakdown of one 
of the routers is not critical for users, as there is typically more than one data packet delivery route. The higher the 
*decentralization level* of a particular system is, the bigger the maximum number of denied components that the system 
can sustain is.

A *decentralized system* implies the presence of many independent participants who maintain its operation together. Note 
that such an approach requires participants to take coordinated actions for sufficiently effective interaction without 
a central party. Decentralization as a phenomenon has many advantages. In order to understand them, one should 
consider the basic concepts and definitions and refer to the history of decentralized systems development.

### Concept of decentralization for information systems
First, we should figure out what an information system is. According to ISO/IEC 2382:2015 standard [1], an information 
system is a system designed for collecting, organizing, storing and processing information and the relevant 
organizational resources. In order to work, an information system requires a database as well as the technical tools 
with the appropriate software for accessing the database and managing the data.

There are two main attributes that distinguish a centralized information system from a decentralized one. The first is 
that in a decentralized system, all components are mandatorily decentralized. “So what?” one might say, “Suppose that a 
centralized service implies that replicas of its database are stored by all its users. Why can’t you call such a system 
decentralized?”

Actually, you cannot because there is the second important feature. It lies in the fact that decentralization “breaks 
down” the core of a system. All the *processes* that used to be indivisible—governance, identity management, asset 
management, participants’ communication, decision-making, storage and processing of information, audit—can now be 
executed by many participants in parallel and independently of one another.

### Difference between decentralized and redundant systems
Redundancy is often utilized to enhance the reliability of a particular system. It implies the addition of excessive 
(backup) components to the system. Such an approach assumes that if one of the components fails, the system will not 
stop working but will rather switch to a backup component. Good examples of redundancy in real life would be the 
duplication of some of the human organs or the executive deputies on a governing body.

According to the above-mentioned description, we provide the following definition. *A redundant system is a system with 
backup components, which are redundant regarding their minimum necessary number and perform the same functions as do the 
basic components.*

Obviously, decentralization implies redundancy mandatorily, but redundancy does not necessarily imply decentralization. 
The point is that redundancy can also be applied in centralized systems. For this, it is enough to add backups of key 
components to a system (e. g., an extra database which replicates the data stored). In a decentralized environment, 
redundancy is the mandatory consequence of the fact that every participant of a particular system has an independent 
set of components.

Based on the definitions of the two systems, we can point out two primary distinctions. The first one is that components 
of a *decentralized system*, unlike those of a redundant one, must not be controlled by a central authority. The second 
one is that redundancy is mandatory in a decentralized system. In a redundant system, it is only applied to improve 
particular operating characteristics and is not mandatory.

## 1.2 History of decentralized systems
As far back as the 1970s, during the search for a more reliable way of storing digital data, the use of decentralization 
principles drew attention. One of the first projects was Usenet [2]. The basic operational principle of this protocol 
was the data exchange between servers using a special algorithm that additionally ensured the synchronization of the 
nodes’ states. In this way, each server was an updated local copy of any other node of the network. If one server 
failed, the system would continue operating because the data copies were stored on any other server. As compared to the 
centralized alternatives available at that time, the Usenet approach made it possible to improve the reliability of data 
storage.

The idea implemented in Usenet protocol indicated the new approach to data storage and synchronization. Naturally, it 
also formed the basis for future attempts to implement a reliable method of data exchange in a decentralized 
environment.

Around that time, the File Transfer Protocol (FTP) was proposed [3]. It allowed users to transfer files to one another 
independently and propelled the emergence of decentralized file-sharing networks and messaging protocols. These began to 
actively develop later in the 1990s and included examples such as Topsites, IRC, Napster, etc.

In the early 1980s, the world saw rapid development of network control protocols TCP/IP [4], which led to the appearance 
of the Internet as we know it today. This fact was a revolution in the world of information, with computers becoming 
able to connect to the global digital space. Business greatly benefited from the transition of processes to a digital 
form, while even governments, for the most part, supported this innovation.

The Internet has become a free network for information sharing and a great example for other areas which have started 
applying the principles of decentralization of data search and processing. Now we refer to them as *open APIs and 
sharing economy* [5]. Their main principles are the direct user interaction and shared use of resources, services, 
content, devices, etc. Further, we will consider how such principles have been applied in accounting systems of 
different types.

### Decentralized file-sharing systems
For file-sharing systems and data storage systems, the decentralized approach implies that different network nodes store 
different file fragments (Fig. 1.1).

[Picture 1.1] - A scheme for distribution of file fragments among

Decentralized applications started to be developed rapidly especially with the invention of services and protocols for 
file sharing (Fig. 1.2).

[Picture 1.2] - Scheme of file sharing in decentralized file-sharing systems

One of the first such services, Napster, provided a way to exchange MP3 files. At that time, recorded music had been 
mostly available on tapes and disks (of course, it required payment). Therefore, Napster became very popular among 
Internet users as it was free and more convenient. Yet, although users interacted on the *peer-to-peer (p2p)* principle, 
the database with the latest version of files was nevertheless stored on a centralized server. This was subsequently 
discovered to be a weakness, which led to the service being shut down following legal pressure from authorities and 
regulators.

Subsequently, other file-sharing networks appeared such as Gnutella, eDonkey2000, DC++, and I2HUB. Further, however, 
most of them came under attack as regulators were able to influence the organizations that stood behind a particular 
service. In 2005, MetaMachine, which had been developing and supporting eDonkey2000, received a dedicated letter from 
the Recording Industry Association of America (RIAA) with a demand to terminate its file-sharing network. As a result, 
activities carried out with eDonkey2000 could not be considered legal, and the company could have borne serious 
responsibility if it had not shut down the service.

The eDonkey2000 project had to be closed. However, this had demonstrated to the world how business and economic 
relations could be changed. The banning and closure of the p2p projects led to the emergence of new projects that began 
developing decentralized models and creating new possibilities for data management: availability, reliability of 
storage, fault-tolerant operation, etc.

In 2001, BitTorrent, a communication protocol for p2p file-sharing, was introduced. It worked quickly and efficiently 
and was not only fault-tolerant but also independent. Initially, a centralized client software was required, but later 
sophisticated torrent clients appeared, while using VPNs (Virtual Private Networks) increased the level of user 
anonymity. BitTorrent is fairly one of the symbols of the decentralized approach, which has successfully worked so far.

In addition to BitTorrent, there are also many alternative solutions for decentralized data storing. One of them is the 
distributed storage IPFS [11]. Like in BitTorrent, the essence of IPFS’s operation is that users do not download files 
from centralized servers but share them with each other. In fact, it is quite similar to the concept of the World-Wide 
Web: in the system, every file is assigned a unique identifier, which is a hash value of it (for further details, see 
3.1), and Git (version control system) is used to trace the history of each file. Such an approach provides the ability 
to have access to the most relevant version of the content and also ensures its authenticity. A file can be searched 
both by an identifier and by human-readable names, which is performed using the decentralized name system IPNS.

### Decentralized data transmission systems
The more actively people have been using the global network, the more pressing the need for privacy has become. In early 
2002, a project called Tor (The Onion Router) [6] was launched. It is a system of proxy servers that allows setting up 
an anonymous network connection protected from having the data transmission traced. Its implementation allowed users 
from around the world to bypass the traffic blocking of local providers and access data while maintaining privacy [7].

Technologies based on decentralization principles received a strong impulse in their development in particular areas. 
For example, in 2004, the first projects using wireless mesh networks in South Africa were launched. The principle of 
their work is that users themselves maintain data transmission channels and perform network packet routing. In such 
networks, nodes “listen” to each other and if a particular node fails, the ones which were connected to the failed node 
seek for alternative nodes to reconnect. This method of organizing network interaction [8] made the Internet more 
accessible in regions where, for various reasons, centralized providers did not deploy their equipment.

### Decentralized decision-making systems
Another interesting application of decentralization are the systems where decision-making is decentralized. Imagine that 
five people put a cake into a shared safe and agreed to eat it only if the majority agrees. Therefore, they split the 
secret of the code lock and distribute its parts between each other. The cake can only be eaten if the majority of 
participants decides to share their part of the secret and unlock the safe (Fig. 1.3). 

[Picture 1.3] - Decision-making by independent parties

Nowadays major firms cannot be managed by one person, and even if they do exist, their effectiveness is quite doubtful. 
For this reason, almost any large company in practice has a board of directors, a countless number of advisors, and 
sometimes even opportunity for employees to participate in decision-making. This approach increases the effectiveness of 
a company through the cooperation of people with different views, different methods for evaluating problems, and 
different approaches to solving them. Thus, the final decision can be considered more objective.

In this way, as the two-way communication between the top management and those in the middle and lower levels grows, the 
performance of an organization typically increases. Nowadays more organizations are turning from the hierarchical 
management model to a more decentralized one, which continues to gain traction.

It is also important not to confuse decentralized systems with parallel computing systems. In both systems there are 
many computers connected in one network. But in the first case, the computational problem is solved by each computer 
anew to achieve independence of the calculation results, and in the second case, the task is divided into subtasks and 
each computer solves its part to reduce the time for obtaining results.

Grid systems use distributed computational resources to reach a common goal (Fig. 1.4). The number of nodes in such a 
system can fluctuate from several machines to hundreds and thousands of workstations.

[Picture 1.4] - Scheme for transferring results of calculations in parallel computing systems

Such an approach was first suggested in 1999 in the publication “The Grid: Blueprint for a new computing infrastructure” 
[9]. That same year the first grid project, SETI@home [10], was launched. Today there are a huge number of similar 
projects such as BOINC, Folding@home, Einstein@Home, etc. Note that the above-mentioned SETI@home project has so far 
been one of the most powerful distributed supercomputers.

### Decentralized payment systems
The next step happened to be the decentralization of payment systems. They were much harder to decentralize for a clear 
reason: people are ultimately anxious about everything directly related to the safety of their money. 

Due to the invention of *money*, the value of private property became much easier to estimate (ability to objectively 
estimate value is one of the fundamental features of money). Money has historically been tied to commodities such as 
gold, cows, furs, shells, cigarettes, etc. The wealth of an individual was based on how much commodity belonged to him. 

Nowadays money has become digital; they have actually become numbers in a database which allow evaluating each others’ 
abilities, power, and status. The problem with this kind of money (so-called *fiat money*) is their non-transparent 
issuance: this process may be performed based on decisions of particular people and not on the overall consensus. Note 
that achieving an overall consensus regarding monetary policy is fairly not a trivial problem.

With the appearance of Bitcoin (the accounting system) in 2009, bitcoin (the base currency) became the first *scarce 
digital asset*. Because of this, the idea to separate money from a state or banks became popular. A similar thing 
happened centuries ago in some of the developed countries with regard to religion and press when they became free 
(almost…) from the state. Nevertheless, the concept of *single national currency* is still explicitly stated in the 
constitutions of many states.

The major question is as follows: is it possible to create an efficient monetary system with initially unlimited 
issuance which is able to simulate the operation of fiat money but is not influenced by particular people? What we can 
say for sure is that the possibility to create digital scarcity (issuance limited with mathematics) and programmable 
rules of work (a constitution guaranteed by cryptography) is revolutionary for many aspects of life and will keep on 
developing and evolving. For this reason, understanding the principles of Bitcoin operation is essential to get yourself 
ready for the new digital world.

In the first volume of the book, we analyze the operating features of a decentralized accounting system with primary 
focus on Bitcoin, since many of the principles which guided its design and implementation are fundamental to any 
decentralized system.

## 1.3 Applying the principles of decentralization
In this subsection, we focus on and formalize the principles of decentralization and specific features of their 
application. These principles have been applied to create well-known and successful applications including data storage 
systems (IPFS), computing systems for load distribution (the BOINC project), mesh networks (Open Garden), 
telecommunications (Tor, I2P), messengers (Tox, BitMessage), and content distribution networks (BitTorrent) as well as 
cryptocurrencies.

### Limitations and issues of centralized systems
The essence of centralized systems is that the management of processes is centralized. In many cases, such an approach 
can provide a system with high efficiency. One of the striking examples is that the protocol rules can be updated simply 
and fast. Suppose a vulnerability is detected in a centralized accounting system, whereas developers discover the source 
of the issue and release an appropriate update. Eventually, all the users who wish to continue using a system have to 
update their software. In this case, the entire process of updating occurs fast and as painless as possible.
> Operation of traditional payment systems
>> * Database is stored on the main server (cloud or cluster)
>> * System is managed in a centralized way 
>> * Users send requests to the system for conducting transactions

