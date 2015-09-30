# Op Codes

### Summary

Bitcoin uses a scripting system to implement transactions. A script is a series of "op codes" and their arguments. For example, 

From the Bitcoin wiki:
>Bitcoin uses a scripting system for transactions. Forth-like, Script is simple, stack-based, and processed from left to right. It is purposefully not Turing-complete, with no loops.
>A script is essentially a list of instructions recorded with each transaction that describe how the next person wanting to spend the Bitcoins being transferred can gain access to them. The script for a typical Bitcoin transfer to destination Bitcoin address D simply encumbers future spending of the bitcoins with two things: the spender must provide:
>
> a public key that, when hashed, yields destination address D embedded in the script, and
>
> a signature to show evidence of the private key corresponding to the public key just provided.
>
> Scripting provides the flexibility to change the parameters of what's needed to spend transferred Bitcoins. For example, the scripting system could be used to require two private keys, or a combination of several, or even no keys at all.
>
>A transaction is valid if nothing in the combined script triggers failure and the top stack item is true (non-zero). The party who originally sent the Bitcoins now being spent, dictates the script operations that will occur last in order to release them for use in another transaction. The party wanting to spend them must provide the input(s) to the previously recorded script that results in those operations occurring last leaving behind true (non-zero).
>
>The stacks hold byte vectors. When used as numbers, byte vectors are interpreted as little-endian variable-length integers with the most significant bit determining the sign of the integer. Thus 0x81 represents -1. 0x80 is another representation of zero (so called negative 0). Positive 0 is represented by a null-length vector. Byte vectors are interpreted as Booleans where False is represented by any representation of zero, and True is represented by any representation of non-zero. 


### High-signal links

https://en.bitcoin.it/wiki/Script

Peter Todd discusses "merklized abstract syntax trees"
https://bitcointalk.org/index.php?topic=255145.msg2757327#msg2757327

Disccusion of OP_CODESEPARATOR
https://bitcointalk.org/index.php?topic=52949.0

Discussion of sidechains
http://diyhpl.us/wiki/transcripts/gmaxwell-sidechains-elements/

Sidechain discussion transcript
http://diyhpl.us/wiki/transcripts/bitcoin-sidechains-unchained-epicenter-adam3us-gmaxwell/

### Low-signal links

Proposed opcode (OP_OP_EXTEND)
https://bitcointalk.org/index.php?topic=24651.0

Proposed opcode (SIGHASH_WITHINPUTVALUE)
https://bitcointalk.org/index.php?topic=181734.20

Proposed opcode (OP_CHECKSIG2)
https://bitcointalk.org/index.php?topic=258931.0

Proposed opcode (OP_DROP)
https://bitcointalk.org/index.php?topic=108423.0

Proposed opcode (OP_EVAL)
https://bitcointalk.org/index.php?topic=46538.0

Proposed opcode (OP_RETURNTRUE)
https://bitcointalk.org/index.php?topic=1106586.msg11773568#msg11773568

Proposed opcode (OP_CHECKSEQUENCEVERIFY)
https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2015-August/010198.html
