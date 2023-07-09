---
title: KIP 003 - Protocol Staking Incentives
status: Active
type: Standards
category: Protocol
author: TandemBikes <thinktankideaists@gmail.com>
team: TandemBikes and Mocolicious
shortDescription: The goal of KIP 003 is create a staking incentive.  Our intention is to borrow from already successful protocol staking mechanisms.
discussions: [Link to a discussion forum, such as GitHub issues or Discord channels.](https://github.com/Kin-Protocol/KIPs/pull/6)
created: 2023-06-15 
updated: 2023-07-09 
---

## Abstract
We're going to use AAVE as a case study because their safety module is the exact kind of incentive system we want to create.
What makes this an effective incentive system is that it encourages participation in securing the protocol and that its simple and transparent.

## Summary
Create a staking incentive, copying AAVE's already successful protocol staking mechanisms.

## Motivation
Makes an effective incentive system that encourages participation in securing the protocol and that is simple and transparent. 

## Rationale
Spends and utilization are difficult to create in cryptocurrency ecosystems, making an effective incentive system that encourages participation in securing the protocol is an incredible use of a users Kin.  Let's get a general sense of how AAVE network bootstapped their staking and some of the loose numbers in the reserve.  With 16 Million AAVE in total reserves to start, emitting 1,110 AAVE per day - the emission percentage is .006875% of Total Reserve per day.  

## Specification
Let's get a general sense of how AAVE network bootstapped their staking and some of the loose numbers in the reserve.  With 16 Million AAVE in total reserves to start, emitting 1,110 AAVE per day - the emission percentage is .006875% of Total Reserve per day.  I would like to propose using the same emission percentage .006875% of Total Reserve released per day.  The supply is a fixed amount, I am proposing 100 Billion Kin.  Protocol staking emissions for AAVE are the only emissions source, and they come from the ecosystem reserve, I am proposing the same be true for Kin.  The AAVE ecosystem reserve is designed to last for only a couple of years currently, although the community can vote to change that. This Kin ecosystem reserve proposition is designed to last for 39.85 years.  The AAVE decentralized governance can decide to use the treasury funds for governance if they choose in future, I would suggest the same for Kin's new decentralized governance.  

Here is my proposal for the KIN Protocol Staking Emissions: 
Kin Staking Reserves will be 100 Billion KIN in reserves to start, multiplied by the emission percentage of .006875% of Total Reserve per day that would mean 6,875,000 million KIN per day in rewards for stakers.
There are 31,536,000 seconds per year.
2,509,375,000 KIN released each year.
79.5 KIN per second.
The unknown will be how much KIN is staked at any given time, but the formula would look like this (79.5 KIN emissions per second x 31,536,000 / current stakes)
So for an example let’s say 200,000,000,000 Kin were staked at any time which is 10% of the total current circulating supply, we get this
79.5 Kin Emissions Per Second x 31,536,000 seconds per year / 200,000,000,000 = .01254 Kin per second for each Kin Staked 
The staking reserves with these numbers lasts for 39.85 years

### Components
A protocol reserve wallet , and a smart contract running the formula I described in the specificaions

### Functionality
The Protocol Staking Incentives smart contract would excute the formula described in the sepcificaion per how many KIN are staked and distrubute KIN rewards from the reserves in the protocol reserve wallet.

### Interface
Interface will be decided by the degov protocol

## Use Cases
Kin holders would utilize this incentive system to secure the protocol and earn Kin.


## Test Cases
See AAVE's active protocol, but we can also setup a wallet with a small portion of the reserves to confirm it's functionality

## Security
There is no minimum or maximum staking period but there is a 10-Day cooldown period and a 2-Day window to unstake 

### Risks
NA

### Mitigations
NA

## Implementation
This is only an improvement proposal so far, no steps beyond creating this proposal have been taken towards acutual implementation. 

## Economics
Described the economics in the specifications section

### Incentives
Incentives are described in the specifications section

### Costs
100 Billion Kin , either from the current KF reserves or crowdfunded by the community.

## Governance
This alligns with the Kin Staking Module proposed by Mocolicious in their new Kin Protocol.

## Community
Makes an effective incentive system that encourages participation in securing the protocol

## Dependencies
Requires the establishment of a protocol reserve wallet , and a smart contract running the formula described in the specificaions.

## References
Please see AAVE's currently functioning staking rewars system as reference

## Copyright
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
