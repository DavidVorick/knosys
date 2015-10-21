##Overview

Proof-of-stake consensus is a power-efficient alternative to proof-of-work
consensus. All modern POS schemes have significant security tradeoffs as
compared to traditional proof-of-work. There are several operational
cryptocurrencies using various forms of proof-of-stake, including centralized
variants.

#### Vocabulary

**DPOS**: Delegated Proof-of-Stake - electing 'delegates' to find blocks.
BitShare's variety of proof-of-stake.

**Nothing at Stake**: A security issue with many proof-of-stake algorithms
where it is costless to create competing blocks. The costlessness means that
there is no reason to choose a single block as the winner of consensus,
instead, numerous competing histories can be created, preventing consensus.

**POS**: Proof-of-stake - abbreviation

**POW**: Proof-of-work - abbreviation - what Bitcoin uses to achieve
distributed consensus, frequently compared against Proof-of-stake systems. 

**Slasher**: A POS algorithm that punishes voters that submit votes for
competing blocks. Slasher is ineffective against people who vote, then sell
their stake, then use the old keys to create competing histories.

**Weak Subjectivity**: Weak subjectivity is an algorithm for requiring a chain
to be substantially (more than 1 block) heavier than the current chain before
reorganizing to accept the other chain. Weak subjectivity solves a variety of
long-term attacks (such as key selling attacks) at the cost of making
bootstrapping a difficult and trust-requried process.

##High Signal Links

2015-03-22 - [On Stake and Consensus](https://download.wpsoftware.net/bitcoin/pos.pdf)

2015-10-06 - [Proof of Stake Summary Wikipedia](https://en.wikipedia.org/wiki/Proof-of-stake)

2015-07-07 - [Proof of Work Analysis](https://eprint.iacr.org/2014/765.pdf)

2015-02-01 - [Proof of Stake Security Issues](https://github.com/ConsensusResearch/articles-papers/blob/master/multistrategy/multistrategy.pdf)

##Low Signal Links

2014-??-?? - [Tendermint Consensus](http://tendermint.com/docs/tendermint.pdf)

2015-08-01 - [Casper POS Algorithm](https://blog.ethereum.org/2015/08/01/introducing-casper-friendly-ghost/)

2014-11-25 - [Nxt Proof of Stake](http://www.scribd.com/doc/248208963/Multibranch-forging#)

2015-05-24 - [Proof of Stake Failures](http://cointelegraph.com/news/114359/the-inevitable-failure-of-proof-of-stake-blockchains-and-why-a-new-algorithm-is-needed)

2014-01-15 - [Slasher: Punitive POS](https://blog.ethereum.org/2014/01/15/slasher-a-punitive-proof-of-stake-algorithm/)

2015-04-08 - [Decentralization and Proof of Stake](https://download.wpsoftware.net/bitcoin/asic-faq.pdf)

2014-11-25 - [Weak Subjectivity](https://blog.ethereum.org/2014/11/25/proof-stake-learned-love-weak-subjectivity/)

2015-03-20 - [Proof of Stake on side chains](https://bitcointalk.org/index.php?topic=997125.msg10835817#msg10835817)

2015-02-02 - [Proof of Stake Security Issues Discussion](https://www.reddit.com/r/Bitcoin/comments/2pvt1e/proof_of_work_proof_of_stake_and_the_consensus/)

2015-08-08 - [Review of Casper, POS Algorithm](http://bytemaster.github.io/2015/08/08/Review-of-Casper-Ethereums-proposed-Proof-of-Stake-Algorithm/)

##Other Forms of Consensus

2015-09-25 - [Stellar Consensus whitepaper](https://www.stellar.org/papers/stellar-consensus-protocol.pdf)

2015-09-25 - [Stellar Consensus Overview](https://medium.com/a-stellar-journey/on-worldwide-consensus-359e9eb3e949)
