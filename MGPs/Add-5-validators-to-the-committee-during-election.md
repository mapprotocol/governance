---
mgp: mgp-0004
title: Add 5 validators to the committee during election
date-created: 2023-01-30
author: Jason (mapdev33), Auroro wu <neoiss>
status: DRAFT
discussions-to: https://forum.mapprotocol.io/t/proposal-add-more-validators-to-the-committee-during-election-2023-01-a-001/4669

---

## Overview

The Validator Committee is responsible for block proposing during each epoch. The current number of validators in Committee is 30 at the moment. 

## Motivation

The previous MGP-0003 suggested adding 10 more spots for new validators to join which was later dequeued because of inadequate votes. The suggested spots in MGP-0003 needs to be reduced to satisfy MAPO security standard. The new MGP-0004 is going to add 5 spots for new validators to join the consensus process.

## Specification

The parameter involved with the change is 

```solidity
   struct ElectableValidators {
        uint256 min;
        uint256 max;
    }
```

 The function that set the change is 

```solidity
    function setElectableValidators(uint256 min, uint256 max) public onlyOwner returns (bool) {
        require(0 < min, "Minimum electable validators cannot be zero");
        require(min <= max, "Maximum electable validators cannot be smaller than minimum");
        require(
            min != electableValidators.min || max != electableValidators.max,
            "Electable validators not changed"
        );
        electableValidators = ElectableValidators(min, max);
        emit ElectableValidatorsSet(min, max);
        return true;
    }
```



The proposed change to the function is 

```solidity
min = 1;
max = 35;
```

which means that there are 45 validators elected during an epoch.

## Implementation

The modification of the validator committee number will be in 

[Election.sol](https://github.com/mapprotocol/atlas-contracts/blob/main/contracts/governance/Election.sol)

## Security Considerations

None.

## License

This work is licensed under the Apache License, Version 2.0.