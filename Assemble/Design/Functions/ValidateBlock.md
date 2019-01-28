# Design Rule
### Prevent Fake PoW
### Prevent Fork
### Eliminate Garbage
### Healthy BlockChain
### PoW-Based
    1. previous's hash: exists & valid?
    2. timestamep: previous's < timestamp < 2 hours + previous's
    3. PoW(on blk): Valid?
    4. txs: Valid?
       S[0] from previous
       S[i+1] = APPLY(S[i],TX[i])
       If no errors until S[n], true. Or, false
       where n is the number of txs and i is an index of one of them.
