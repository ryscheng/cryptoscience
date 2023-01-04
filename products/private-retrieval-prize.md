
# IPFS private retrieval prize

## Summary

We want private retrieval in IPFS implemented and widely used

## Goals

Candidate dimensions of evaluation:
- Specification for implementing compatible implementations 
  - Great: Other groups/implementations have implemented the spec
  - Good: spec is approved by the IPFS standards committee
  - Okay: spec is defined somewhere
- Implementation
  - Great: Production-quality implementation is merged into a popular IPFS implementation
    - [kubo](https://github.com/ipfs/kubo)
    - [go-ipfs-http-client](https://github.com/ipfs/go-ipfs-http-client)
  - Good: Implementation is merged into a minor IPFS implementation (based on share of users)
  - Okay: Implementation released in an unused (new) implementation
- Usage: if privacy-mode is opt-in (e.g. via feature-flag)
  - Based on how many users are leveraging the tool
    - Number of users per day/month
    - Number of read/write operations per day/month
    - Fraction of total IPFS usage over privacy-preserving protocols
    - Retention of privacy-preserving usage
    - Percentage of "high-value" users using it by default (e.g. IPFS gateways)
- Performance - ideally with standardized benchmarks
  - Latency of operations
  - Throughput of operations
  - Read vs write operations
- Security Goals
  - indistinguishability
  - differential privacy
  - k-anonymity
- Threat Model
  - untrusted vs anytrust servers
  - global vs local adversary
  - active vs passive adversary
- Marginal success
  - Are you the first to reach a point?
  - Do we pay a full or discount reward to the second to reach a point?

## Evaluations

1. Security Expert Evaluation: for security goals + threat model
2. Automated Evaluation: for performance + usage
  - [ProbeLab](https://research.protocol.ai/groups/probelab/)
  - [Testground](https://github.com/testground/testground/)
  - [IPFS benchmarks](https://github.com/ipfs/benchmarks)
  - [IPFS profiling](https://github.com/ipfs-inactive/ipfs-performance-profiling)
3. Implementer Evaluation: for pull requests and standard process

## Rewards

In our 6-dimensional space, how do we effectively allocate rewards?

## Meta-evaluation: Bounty/Prizes vs Grants

How does this compare to the status quo / alternative?
- after some RFP-14 grants, select the most promising research directions
- distribute implementation grants 
- measure impact (e.g. how much usage we see)
- funder makes strategic decisions on how to allocate future implementation grants

Ways to evaluate:
- A/B test - difficult to do - requires more thinking
  - If different RFPs, then the nature of the problem could yield different results
  - If same RFP, launching 2 different incentives simultaneously can conflict with each other
- Analytically - e.g. via game theory

## Outcome Scenarios

Intuitions:
- If "how" something should be done is more narrow and straight-forward, I'd expect grants to win
- If "how" something should be done is multi-dimensional with a lot of unknowns, I'd expect prizes to do better. 
- In grants, it's up to the funder to make both strategic and cost-saving decisions.
  - In prizes, it's up to the participants and their investors
- Grants fall susceptible to perverse incentives of budget over-runs
  - Think public infrastructure or defense spending
  - Once you've sunk cost into a particular direction, it becomes harder to pivot
- Prizes - only paying for success conditions that have value to you

1. Multiple successful implementations 
2. Participants reach less useful 
3. Noone gets anywhere
  

