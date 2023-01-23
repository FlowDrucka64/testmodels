# Lightning

## First Transcation
![PCN](figs/lightning1.JPG)

## State Change
![PCN](figs/lightning2.JPG)

## PCN
![PCN](figs/lightning3.JPG)
![PCN](figs/lightning4.JPG)
![PCN](figs/lightning5.JPG)
![PCN](figs/lightning6.JPG)
![PCN](figs/lightning7.JPG)


## Wormhole
![PCN](figs/lightning8.JPG)

## Privacy
![PCN](figs/lightning9.JPG)


## Fulgor
First Alice distrbutes keys (and ZKPs) to all parties.
Each intermediate party can open their lock when the party to the right has opened theirs.


![PCN](figs/lightning11.JPG)

## Recap
![PCN](figs/lightning12.JPG)
![PCN](figs/lightning13.JPG)

# Blitz
Try to do it in "one round".
## Attempt 1
![PCN](figs/blitz1.JPG)
## Attempt 2
![PCN](figs/blitz2.JPG)
## Attempt 3
![PCN](figs/blitz3.JPG)

## Pay or Revoke Paradigm
![PCN](figs/blitz4.JPG)
### Successful
![PCN](figs/blitz5.JPG)
### Refund
![PCN](figs/blitz6.JPG)

## Lightning vs. Blitz
![PCN](figs/blitz7.JPG)


# Thora
![PCN](figs/thora1.JPG)
## Setup
![PCN](figs/thora2.JPG)
![PCN](figs/thora3.JPG)

## Success
![PCN](figs/thora4.JPG)

## Revoke
![PCN](figs/thora5.JPG)

## Take home
![PCN](figs/thora6.JPG)

# Virtual Channels
## Idea
![PCN](figs/vc1.JPG)
![PCN](figs/vc2.JPG)
## Take home
![PCN](figs/vc3.JPG)


# Payment Channel Hubs
## Idea
![PCN](figs/pch1.JPG)
## Atomicity
![PCN](figs/pch2.JPG)
## Unlinkability
![PCN](figs/pch3.JPG)
## PCH with Fulgor
![PCN](figs/pch4.JPG)
![PCN](figs/pch5.JPG)

## Adaptor Signatures
![PCN](figs/pch6.JPG)
![PCN](figs/pch7.JPG)


## PCH with Adaptor Signatures
### First attempt
![PCN](figs/pch8.JPG)

### Privacy Issue
![PCN](figs/pch9.JPG)

### Privacy Solution
![PCN](figs/pch10.JPG)

### Randomizable Puzzle
![PCN](figs/pch11.JPG)

## A²L Protocol
![PCN](figs/pch12.JPG)

### Griefing Protection
![PCN](figs/pch13.JPG)

### Take Home
![PCN](figs/pch14.JPG)



# Scaling overview
![PCN](figs/scale1.JPG)

## Idea
![PCN](figs/scale2.JPG)
## Problem
![PCN](figs/scale3.JPG)
## Solution (?)
![PCN](figs/scale4.JPG)


# Watchtowers
## Problem: Incentive
![PCN](figs/watchtower1.JPG)

## Solution: Collateral
![PCN](figs/watchtower2.JPG)

## Cerberus Channels
![PCN](figs/watchtower5.JPG)

### Notation
![PCN](figs/watchtower3.JPG)

Output (a+b) can either be spent by having the signature of A and waiting t or by having a multisig of A and B.

### Nonworking soltion (1/4)
Alice and WT can collude to scam bob.
Alice can spend output just after t. Bob would not be able to publish the penalty since the output is already spent.

![PCN](figs/cerb5.JPG)


### Nonworking soltion (2/4)
(Change to previous approach: Penalty depends on output controlled by bob instead of alice)

Alice and Bob can collude to scam WT.
Publish commitment + penalty right away.  WT has racecondition on the revocation.

![PCN](figs/cerb4.JPG)

### Nonworking soltion (3/4)
(Change to previous approach: Add timelock to the input of the penalty)

Alice and bob can collude to scam WT.

Alice and bob agree to spend earlier output (not by revocation) making the revocation TX invalid.Then Bob can publish the penalty TX and WT cannot do anything about it.

![PCN](figs/cerb3.JPG)

### Nonworking soltion (4/4)
(Change to previous approach: Multisigs at outputs of commitment. Add timelock to bob's output -> cant send penalty right away (give WT time to react))

Alice and WT can collude to scam bob.

WT reclaims, Alice spends earlier tx.

![PCN](figs/cerb2.JPG)


### Working solution
![PCN](figs/cerb1.JPG)


# Watchtower Committee
![PCN](figs/watchtower6.JPG)

## Challanges
![PCN](figs/watchtower7.JPG)

## Solution
![PCN](figs/watchtower8.JPG)
![PCN](figs/watchtower9.JPG)
![PCN](figs/watchtower10.JPG)
![PCN](figs/watchtower11.JPG)
![PCN](figs/watchtower12.JPG)

## Incentives
![PCN](figs/watchtower13.JPG)

Why assist to close honsetly?

### Collateral
![PCN](figs/watchtower14.JPG)
![PCN](figs/watchtower15.JPG)
![PCN](figs/watchtower16.JPG)
![PCN](figs/watchtower17.JPG)

### Why assist to close?
![PCN](figs/watchtower18.JPG)

### Why request to close?
![PCN](figs/watchtower19.JPG)

### Brick advantages
![PCN](figs/watchtower20.JPG)




# Sharding
## Requirements
![PCN](figs/shard5.JPG)
### Persistence
![PCN](figs/shard1.JPG)
### Consistency
![PCN](figs/shard2.JPG)
### Liveness
![PCN](figs/shard3.JPG)
### Scalability
![PCN](figs/shard4.JPG)

## The model
![PCN](figs/shard24.JPG)

## Boundaries
![PCN](figs/shard6.JPG)
![PCN](figs/shard7.JPG)
![PCN](figs/shard8.JPG)
![PCN](figs/shard9.JPG)

## Roadmap
![PCN](figs/shard10.JPG)
![PCN](figs/shard11.JPG)
![PCN](figs/shard12.JPG)
![PCN](figs/shard13.JPG)
![PCN](figs/shard14.JPG)
![PCN](figs/shard15.JPG)
![PCN](figs/shard16.JPG)
![PCN](figs/shard17.JPG)

## The shardinc crux
![PCN](figs/shard18.JPG)
![PCN](figs/shard19.JPG)
![PCN](figs/shard20.JPG)
![PCN](figs/shard21.JPG)

## Evaluation
![PCN](figs/shard22.JPG)

## Recap
![PCN](figs/shard23.JPG)


# Rollups
![PCN](figs/ru1.JPG)

## ZK-rollups
![PCN](figs/ru2.JPG)

## Optimistic rollups
![PCN](figs/ru3.JPG)


# Current research topics
![PCN](figs/re.JPG)
