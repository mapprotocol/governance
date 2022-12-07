---
mgp: <to be assigned>
title: <CGP title>
date-created: <date created on, in ISO 8601 (yyyy-mm-dd) format>
author: <a list of the author's or authors' name(s) and/or username(s), or name(s) and email(s), e.g. (use with the parentheses or triangular brackets): FirstName LastName (@GitHubUsername), FirstName LastName <foo@bar.com>, FirstName (@GitHubUsername) and GitHubUsername (@GitHubUsername)>
status: <DRAFT | PROPOSED | EXECUTED | EXPIRED | WITHDRAWN>
discussions-to: <link to discussion on https://forum.maplabs.io/>
governance-proposal-id: [if submitted]
date-executed: [if executed] <date created on, in ISO 8601 (yyyy-mm-dd) format>
---
## Overview

This is the suggested template for new MGPs.

Note that a MGP number will be assigned by an editor. When opening a pull request to submit your MGP, please use an abbreviated title in the filename, `MGP-draft_title_abbrev.md`.

### Status
- DRAFT = Feedback collection
- PROPOSED = The governance proposal was submitted to the network
- EXECUTED = The governance proposal was executed on the network
- EXPIRED = The governance proposal expired
- WITHDRAWN = The governance proposal is withdrawn before being submitted on the network

Describe the issue that motivates this MGP. It should indicate all parameters that are being changed and why doing so is important.

Explain what benefits the enhancement this change will bring. To the extent possible, enumerate use cases affected by this MGP.

Once the proposal is successfully proposed on chain, update this file so that the title number matches the proposal ID.

## Abstract

A short (~200 word) description of the technical issue being addressed.

## Motivation

The motivation is critical for MGPs that want to change the MAPO protocol. It should clearly explain why the existing protocol specification is inadequate to address the problem that the MGP solves. MGP submissions without sufficient motivation may be rejected outright.

## Specification

The technical specification should describe the syntax and semantics of any new feature. 

## Proposed Changes

Fill out the following template for each transaction in the proposal

1. Description of transaction 1

- Destination: A human readable description of the address and method being called
- Data: A human readable description of the transaction data
- Value: How much MAPO is being sent, and why?

## Rationale

The rationale fleshes out the specification by describing what motivated the design and why particular design decisions were made. It should describe alternate designs that were considered and related work, e.g. how the feature is supported in other languages. The rationale may also provide evidence of consensus within the community, and should discuss important objections or concerns raised during discussion.

## Backwards Compatibility

All MGPs that introduce backwards incompatibilities must include a section describing these incompatibilities and their severity. The MGP must explain how the author proposes to deal with these incompatibilities. MGP submissions without a sufficient backwards compatibility treatise may be rejected outright.

## Test Cases

Test cases for an implementation are mandatory for MGPs that are affecting consensus changes. Other MGPs can choose to include links to test cases if applicable.

## Implementation

The implementations must be completed before any MGP is given status "Final", but it need not be completed before the MGP is accepted. While there is merit to the approach of reaching consensus on the specification and rationale before writing code, the principle of "rough consensus and running code" is still useful when it comes to resolving many discussions of API details.

## Security Considerations

All MGPs must contain a section that discusses the security implications/considerations relevant to the proposed change. Include information that might be important for security discussions, surfaces risks and can be used throughout the life cycle of the proposal. E.g. include security-relevant design decisions, concerns, important discussions, implementation-specific guidance and pitfalls, an outline of threats and risks and how they are being addressed. MGP submissions missing the "Security Considerations" section will be rejected. A MGP cannot proceed to status "Final" without a Security Considerations discussion deemed sufficient by the reviewers.

## License

This work is licensed under the Apache License, Version 2.0.