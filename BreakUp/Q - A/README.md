# MINING ISSUES
### GENESIS
    - CREATE
      > FROM GENESIS.JSON: geth init genesis.json
      > FROM SOURCE CODE[core/genesis.go]: geth console
    - ALLOC ACCOUNT
      > reflected into genesis block, reflected into statedb?
### MINING CYLCE
    TX COLLECT, TX SORT, TX VALIDATE, BLK CREATE, BLK VALIDATE, BLK BROADCAST, BLK CONFIRM
### TX CYCLE
    SIGNED, BROADCASTED, VALIDATED, CONFIRMED?
    - SIGNED?
      > txmsg = txdata(sender, receiver, amount, time, ...) + sign
    - WHAT SIGN IS?
      > sign = privatekey + secretkey + txhash(based on tx time and/or tx data)
    - VALIDATED?
      > sign + publickey?
      > publickey in statedb
    - CONFIRMED? 
      > "tx confirmed" is "block confirmed"
### HASH POWER
    - mining pool?
      > Reward(node) = Reward(blk) * hashpower(node)/hashpower(sum of nodes contributed to a blk gened.)
      > randomly rewarded -> small, but regularly rewared
      > Avg block generation time on a node: 2 years
      > ?: PoW work is distributed on several nodes or not?
      > ?:
    - A mining pool with 30% hashpower?
      >
    - hashpower & hashrate?
      >
    - what guarantes 15s block time?
      >
### GHOST2Uncles
    Blk TIme >> Blk Propogation Time :  Small Stale Rates or Zero Stale Rates
    High Blk Occurance Rate:  Fork, Collision
   * Short Block Time -> High Stale Rates -> Traffic Amplification -> Security Issue: Longest 2 Widest
   * Fast Confirmation -> Fuzzy2Clear(Hashpower's Influence Over Mining) -> Centralization: Reward 2 Stale
    
    - What if uncles are not rewarded?
### Uncles
    U: Uncle, B: The Block
   * 7 generations
   * direct child of B's k-th ancester, where 2 <= k <= 7
   * valid blk header, but not need valid blk
   * At Most X Uncles for B, At Least 0
   * B's uncles =/= B's ancesters' uncles
   * 93.75% for U miner, 3.125% for B miner
   
    Pros
   * High Security: Miners Do Not Know If Mining Main or Stale.
   *
### STATEDB: 
# SECURITY ISSUES
### 
