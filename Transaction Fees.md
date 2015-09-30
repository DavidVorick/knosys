##Overview

Transaction fees are coins in transactions that are given to miners when the transaction is mined into a block. The transaction fee is given to the miner, which provides an incentive for the miner to place the transaction into a block. There is a non-zero cost associated with including a transaction into a block. Blocks with transaction propagate through the network slower than blocks without transactions. Slower propagating blocks are at higher risk of being orphaned. Infrastructure such as [IBLTs] and [Near Blocks] help reduce the orphan rate on larger blocks, and therefore help reduce the cost of adding a transaction to a block.

Because of the block size limit, only a finite number of transactions can be included into a block. Transaction fees establish a way to pick which transactions should go into a block. Transactions with insufficient fees may get stuck on the network, which can be espeically problematic when mempools never prune the transaction and also never accept a double spend of the outputs in the unconfirmed transaction. Policies such as [Replace By Fee] and [Child Pays for Parent] affect transaction circulation. Wallets can avoid making destined-to-fail transactions by participating in [Fee Discovery].

Fees are added to transactions by having the sum of the outputs of the transaction be less than the sum of the inputs of the transaction. People have infrequently added an absurd transaction fee to a transaction by miscalculating the outputs. The transaction fee cannot be determined by looking at the transaction alone, additional information about the outputs being spent is required. These shortcomings have led to proposals such as [OP_FEE] and [OP_CHECKFEE].

The current block reward is 25 Bitcoins. Eventually, this reward will fall heavily towards 0. With a 0-value block reward, the primary source of income for miners becomes transaction fees. This can lead to issues such as [Fee Sniping] and [Underfunded Mining].

Links on this page include the topics of 'transaction relay policy', 'miner income', 'network fee policy', 'replace-by-fee,' 'fee sniping', 'fee sharing', 'OP_FEE' 'child-pays-for-parent', 'fee discovery'.

#### Vocabulary

**CPFP/CP4P**: Child Pays For Parent - a child transaction with high fees can incentivize miners to add the unconfirmed parent transaction to a block.

**Fee Sniping**: Miners try to re-mine the most recent block so that they may steal the fees in the block.

**RBF**: Replace By Fee - the outputs of an unconfirmed transaction are double-spent in a new transaction with higher miner fees.

##High Signal Links

2015-02-12 - [Replace by fee v0.10.0rc4] (http://lists.linuxfoundation.org/pipermail/bitcoin-dev/2015-February/007404.html)

2013-02-24 - [Fee backlogs discourage fee sniping] (http://lists.linuxfoundation.org/pipermail/bitcoin-dev/2013-February/002186.html)

2013-04-14 - [Funding network security in the future] (https://bitcointalk.org/index.php?topic=176684.0)

2015-05-26 - [First Seen Safe Replace By Fee] (http://lists.linuxfoundation.org/pipermail/bitcoin-dev/2015-May/008248.html)

2014-04-28 - [Replace-by-fee scorched-earth without child-pays-for-parent] (http://lists.linuxfoundation.org/pipermail/bitcoin-dev/2014-April/005620.html)

##Low Signal Links

2015-06-29 - [Replace by fee deployment schedule] (http://lists.linuxfoundation.org/pipermail/bitcoin-dev/2015-June/009253.html)

2013-10-24 - [Have miners announce their required fees] (http://lists.linuxfoundation.org/pipermail/bitcoin-dev/2013-October/003421.html)

2015-07-11 - [Random block size to facilitate a fee market] (https://bitcointalk.org/index.php?topic=1117914.0)

2014-08-07 - [SIGHASH_ANYONECANPAY extra inputs DoS attack] (http://lists.linuxfoundation.org/pipermail/bitcoin-dev/2014-August/006438.html)

2015-06-10 - [SPV Fee Discovery mechnaism] (http://lists.linuxfoundation.org/pipermail/bitcoin-dev/2015-June/008549.html)

2014-04-24 - [Replace by fee game theory] (http://lists.linuxfoundation.org/pipermail/bitcoin-dev/2014-April/005504.html)

2013-04-29 - [OP_FEE - explicit transaction fees] (https://bitcointalk.org/index.php?topic=191003.0)

2013-11-22 - [OP_CHECKFEE - an opcode indicating the transaction fee] (so utxo can remain unknown to hardware wallets): https://bitcointalk.org/index.php?topic=343234.0

2013-09-23 - [Near Blocks for Fee Estimation] (http://lists.linuxfoundation.org/pipermail/bitcoin-dev/2013-September/003275.html)

2015-02-12 - [Facing Replace By Fee] (http://sourceforge.net/p/bitcoin/mailman/message/33405247/)

2015-09-04 - [Fee pressure on utxo settling] (http://lists.linuxfoundation.org/pipermail/bitcoin-dev/2015-September/010909.html)

2011-06-06 - [Future fee policy for relaying and mining] (https://bitcointalk.org/index.php?topic=12625.0)

2012-06-15 - [Fee policy for relaying and mining] (http://lists.linuxfoundation.org/pipermail/bitcoin-dev/2012-June/001533.html)

2015-05-28 - [Replace by Fee is Harmful] (https://www.reddit.com/r/Bitcoin/comments/30lxo4/replace_by_fee_a_counter_argument_by_mike_hearn/)

2015-06-19 - [F2Pool enabled Full RBF] (https://www.reddit.com/r/Bitcoin/comments/3ae2e1/peter_todd_f2pool_enabled_full_replacebyfee_rbf/)

2015-05-07 - [Block size increase] (http://lists.linuxfoundation.org/pipermail/bitcoin-dev/2015-May/007880.html)

2011-09-25 - [Network-Adjusted transaction fees] (https://bitcointalk.org/index.php?topic=45665.0)

2015-06-24 - [Fees are Inevitable] (https://www.reddit.com/r/Bitcoin/comments/3b0593/to_fork_or_not_to_fork/cshphic)

2014-06-09 - [Earn 1% more by mining replace-by-fee] (https://bitcointalk.org/index.php?topic=645120.0)

2015-06-18 - [Replace by Fee Cuts Waste - Reddit Discussion] (https://www.reddit.com/r/Bitcoin/comments/3aawqp/this_is_consensus/csb92so)

------

##### Contributors

David Vorick
