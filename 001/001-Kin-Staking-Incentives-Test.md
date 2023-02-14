
---
title: Kin Staking Incentives Test
status: Proposed
author: Andrew Mocol (@mocolicious)
shortDescription: 
discussions: TBD
created: 2023-02-11
---


## Summary

This proposal is an initial test proposal for the governance system to allocate and amount of 1 billion kin to the staking module to test it with a real amount of staking incentives.

## Motivation

The staking system was put in place with the idea that a healthy amount of incentive woud be required to keep people active in the governance process.  To enourage maximum participation of community members they should be rewarded for signalling into the module and the ecosystem benefits from reduced potential sell pressure since much of the kin will locked away in the staking module.

## Specification

The staking amount would distributed over the course of a 6 month period.  So the protocol would need to calculate the APY based on a linear model that bases a fixed APY rate on time adjusted math calculating based on the time of locking started. The lower higher the utilization, the lower the APY.

## Security

Since this requires an additional SPL component with exact math, it will require an audit prior to entering the final review

## Implementation

TBD

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
