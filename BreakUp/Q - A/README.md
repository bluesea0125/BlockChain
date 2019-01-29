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
      >
    - A mining pool with 30% hashpower?
      >
    - hashpower & hashrate?
      >
    - what guarantes 15s block time?
      >
### STATEDB: 
# SECURITY ISSUES
### 
