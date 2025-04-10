# Features Config v2

## Available

### Hidden [Highest priority]
Control whether to show or hide the feature, ignoring the whitelist
- 0: visible for all addresses
- 1: visible for only whitelisted addresses
- 2: hidden for all addresses

### Whitelist [Second priority]
Controls whether the feature is available for a specific address. `available` is true if the address is in the whitelist. When the whitelist is empty, `available` is true for all addresses. When hidden is true, this control is invalid.
- ["0x1234", "0x5678"]: only "0x1234" and "0x5678" can use the feature
- []: all addresses can use the feature

## Id
Currently, it is just used for Morpho vaults, and it is used as the id of the Morpho vault.

## Action
Controls the action that the feature manages.
- general
- deposit
- withdraw
- rewards
- etc.
