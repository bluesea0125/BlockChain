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
### GHOST
   * Short Block Time -> High Stale Rates -> Traffic Amplification -> Security Issue: Longest 2 Widest
   * Fast Confirmation -> Stale Blk Overflow -> Centralization Issue: Reward 2 Stale(7/8 4 Uncles & 1/8 4 Nephew...)
   * If Blk Propogation Time << Blk TIme, Small Stale Rates or Zero Stale Rates
### STATEDB: 
# SECURITY ISSUES
### 
