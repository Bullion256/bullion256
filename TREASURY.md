# Bullion256 Treasury (Main Network)

This document defines the consensus-enforced treasury design for Bullion256 (BUL).

This is NOT Signet.
This is the Bullion256 main production network.

-----------------------------------------------------------------------

## Treasury Policy

• Consensus Enforced: YES  
• Treasury Percentage: 10% of block subsidy  
• Script Type: P2WPKH (SegWit v0)  
• Network: Bullion256 Main Chain  
• Enforcement Location: validation.cpp (ConnectBlock)

Any block that does not include the correct treasury output
with the exact required amount is INVALID.

-----------------------------------------------------------------------

## Official Treasury Address

bul1q37fsw2457hy2jsjdnx29h3tjexkzqz67cwxqx4

Witness Program (v0):

8f93072ab4f5c8a9424d99945bc572c9ac200b5e

ScriptPubKey (consensus enforced):

OP_0 8f93072ab4f5c8a9424d99945bc572c9ac200b5e

Hex form:

00148f93072ab4f5c8a9424d99945bc572c9ac200b5e

-----------------------------------------------------------------------

## Enforcement Logic

Inside validation.cpp:

Treasury amount required:

expectedTreasury = GetBlockSubsidy(height) / 10

Validation rule:

• Treasury output must exist
• Treasury output must match the exact witness program above
• Treasury output value must equal 10% of subsidy
• No rounding tolerance
• No alternative scripts accepted

If any condition fails:

BlockValidationResult::BLOCK_CONSENSUS
Reject reason: bad-cb-treasury-amount

-----------------------------------------------------------------------

## Monetary Model

Initial Subsidy: 50 BUL  
Halving Schedule: Bitcoin-style interval  
Tail Emission: 1 BUL minimum  

Treasury always receives 10% of subsidy
regardless of halving stage.

Example at 50 BUL subsidy:

Miner: 45 BUL  
Treasury: 5 BUL  

-----------------------------------------------------------------------

## Governance

Treasury funds are controlled by the private key
corresponding to the address above.

Key rotation requires:

• Spending treasury funds to a new address
• Updating consensus code
• Hard fork (if script changes)

-----------------------------------------------------------------------

## Status

Treasury: ACTIVE  
Consensus Enforcement: ACTIVE  
Script Type: P2WPKH (v0)  
Network: Bullion256 Main Chain  
Genesis Height: 0  
Current Height: dynamic

-----------------------------------------------------------------------

This document reflects the live consensus rules
compiled into the Bullion256 daemon.
