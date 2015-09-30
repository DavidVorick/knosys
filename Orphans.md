#Orphans
###jw

##Requesting parents for orphan transactions
gzzrmtp5 2015-08-29T20:57:02+00:00
An orphan transaction is a transaction where some of the parents are missing.  This means that it cannot be added to the memory pool, since there is no way to verify those inputs...[Something like the "getheaders" message would make this more efficient.](https://bitcointalk.org/index.php?topic=1065390.0)
>bitcointalk bitcoin orphan-transactions orphans transactions tier-nolan tiernolan year-2015 hash-map transaction-chaining proposal scalability scaling transaction-archival

##Adopting block chain orphans
dx6epha4 2015-08-29T02:08:31+00:00
It seems to me that discarding orphan blocks outright loses their potential utility in hardening the byzantine voting on the transaction log.  ie work went into them, but currently they are given no weighting in the chain length [(AFAIK).](https://bitcointalk.org/index.php?topic=194573.0)
>bitcointalk bitcoin adam3us adam-back mining orphans orphan-blocks year-2013 gmaxwell first-past-the-post-race network-latency bandwidth tiernolan spv p2pool

##How small blocks make deliberate orphan mining more costly
udhgolei 2015-08-30T14:51:44+00:00
In the low-subsidy future fees will be the main source of income forminers. Thus in some circumstances large miners may even have a reason to delibrately try to mine a block that would orphan the current best block. [A simple example would be](http://lists.linuxfoundation.org/pipermail/bitcoin-dev/2013-February/002186.html)
>bitcoin bitcoin-dev mailing-list email year-2013 gmaxwell petertodd fee-sniping fees orphans orphan-blocks orphan-block mining fee-snipe miners low-subsidy nlocktime-immaturity nlocktime-immature block-size max-block-size

##What is the longest blockchain fork that has been orphaned to date?
e42xnwgz 2014-11-15T23:05:23+00:00
The Value Overflow incident seems to be the longest ever blockchain split. The problem with blockchain forks is that once they are resolved the only trace they leave is a log entry. [The problem is quite evident:](http://bitcoin.stackexchange.com/questions/3343/what-is-the-longest-blockchain-fork-that-has-been-orphaned-to-date/4638#4638)
>stackexchange bitcoin blockchain orphans orphan-blocks blocks reorgs reorg orphaned-blocks

##How to avoid getting stuck in orphaned chains?
5qzguibs 2014-11-16T22:49:32+00:00
I'm manually parsing the blockchain using bitcoind, calling getblock(), then processing, then moving to the nextblockhash. However, I can quite easily get stuck in a orphaned block, or chain of blocks. [What can I do to prevent this?](https://bitcointalk.org/index.php?topic=364191.0)
>bitcointalk bitcoin reorgs getblock orphans reorganizations kjj getblockhash getblockcount blocknotify reorg

##Propagating orphan block headers
wvt5x77l 2015-08-29T17:45:21+00:00
According to the official protocol rules, when a node receives a block that extends an orphan branch (but doesn't make it the main chain), the client simply stores the block.  It doesn't relay it. [But!](https://bitcointalk.org/index.php?topic=219171.0)
>bitcointalk bitcoin tier-nolan tiernolan proposal orphans blockheaders propagation relaying relay partitions splits network-splitting network-split orphan-branch year-2013
##How a floating blocksize limit inevitably leads towards centralization
hy3wpuon 2015-08-29T17:21:28+00:00
The idea that miners have a strong incentive to distribute blocks as widely and as quickly as possible is a serious misconception. The optimal situation for a miner is if they can guarantee their blocks would reach just over 50% of the overall hashing power, but no more. [The reason is orphans.](https://bitcointalk.org/index.php?topic=144895.0)
>bitcointalk bitcoin petertodd year-2013 max-block-size block-size incentives centralization decentralization orphans orphan-rate empty-blocks transactions scalability scaling mining-incentives

##Reducing the chance for random reversal
xm64ryfx 2015-08-29T17:48:33+00:00
This allows the network settle on which block to orphan much faster. [For example,](https://bitcointalk.org/index.php?topic=244682.0)
>bitcointalk bitcoin tier-nolan tiernolan etotheipi jl2012 subchains sub-chains confirmations reorgs reversals orphan-rate orphans alt-chains proposal scaling scalability mining

##Detecting and handling fork events
vzyfotyu 2015-08-29T17:57:52+00:00
Detecting, Precations, Reacting. [Orphan rate will increase](https://bitcointalk.org/index.php?topic=262281.0)
>bitcointalk bitcoin tier-nolan tiernolan proposal forks forking fork-events headers blockheaders blockchain tree tree-extension orphan-branches orphans relaying nodes year-2013

##Chain reorganization
edlwz5mo 2014-11-15T23:05:45+00:00
Excluded blocks become [orphans.](https://en.bitcoin.it/wiki/Chain_Reorganization)
>bitcoin wiki reorgs reorg reorganization orphans orphan-blocks orphaned-blocks

##Sidechains talk, Matt Corallo
vr5k4jrx 2015-03-09T03:12:54+00:00
What happens when the two way peg is part of an orphan block on the original blockchain?[Answer](http://diyhpl.us/wiki/transcripts/mit-bitcoin-expo-2015/matt-corallo-sidechains/)
>mit bitcoin mit-bitcoin-expo-2015 mit-bitcoin-expo conference transcript matt-corallo thebluematt bluematt blockstream blockchain sidechains sidechain soft-forks hard-forks orphans orphan-blocks

#Decoupling transactions and POW
fy5nog42 2015-08-29T17:34:53+00:00
Low signal link on [orphans](https://bitcointalk.org/index.php?topic=179598.0)
>bitcointalk bitcoin tier-nolan tiernolan proposal proof-of-work blockheaders pow-header blocks sub-chain sub-chain-blocks subchains subchain soft-fork orphan-rate sub-chain-links subchain-links backwards-compatible block-rate scaling scalability confirmations confirmation-time year-2013

