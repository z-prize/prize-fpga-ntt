# Accelerating NTT Operations on an FPGA

  

Prize Sponsor: Polygon

Prize Architect: DZK

## Prize Description

### Summary

  

Number-theoretic transformations (NTT) are essential building blocks for zero-knowledge proof protocols based on error-correcting codes, such as STARK and Plonky2. This prize will focus on using AMD Xilinx Varium C1100 Blockchain Accelerator Card, a card tailored for blockchain acceleration, to accelerate NTT in Polygon Zero’s Goldilocks field.

### Optimization Objective (1-sentence)

  

Compute radix-2 NTT over the Goldilocks field (modulo 2^64 - 2^32 + 1) with lowest latency, adjusted by the power consumption.

### Constraints

  

-   Participants need to register, and we will admit participants who already have experience with the FPGA design toolchain. AMD can provide access to devices. Participants in universities should already have access to the design toolchain from the school.
    

-   The code will be open-sourced at the end of the competition under a permissive license. Contestants can choose between Apache 2.0 and/or MIT. For the competition’s fairness, code must remain private throughout the competition.
    
-   Two FPGA cards may be used in the second milestone of the competition. In the first milestone, only one card may be used.
    
-   Submissions must include documentation, in English, sufficient to understand the optimization approach.
    

  

## Timeline

  

June 10 - Competition begins

August 15 - Phase 2 begins

September 10 - Competition completes

  
  

## Judging

  

The competition will consist of two parts.

  

1.  First, competitors should implement NTT that is functional, so that it can reach the following scale:
    

-  First milestone: 2^18
    
-  Second milestone: 2^24
    

2.  All competitors that build correct implementations in the first phase will proceed to the performance competition, where the goal is to implement NTT with the lowest latency.
    

-  This will be evaluated in the first 2.5 months. Teams that pass the second milestone enter the performance competition.
    
-  In the performance competition, one can use many cards. We consider the latency, adjusted by the power consumption.
    

  

Contestants for the prize will be selected based on their prior documented experience and academic achievement. Admission to the competition will be determined by a committee consisting of representatives from -

  

1.  Prize sponsor (Polygon)
    
2.  Prize architect (DZK)
    
3.  Technology partner (AMD Xilinx)
    

  

Submissions will be analyzed for both correctness and performance.

### Correctness

  

We will provide a set of test input/output pairs so that the competitors can sanity check the correctness of their code.

  

The final correctness of the submission will be tested using randomly sampled test inputs/outputs that are not disclosed to the competitors during the competition in addition to the test input/output distributed to the competitor. Submissions failed in any test cases will be judged as incorrect and lose the opportunity to win the prize.

### Performance

  

The speed competition (Phase 2) will be awarded according to latency (adjusted by power consumption).

### Hardware & Benchmarks

  

We will provide a reference implementation that consists of a high-level synthesis for NTT sufficient to 2^12. This covers the general logic but needs efforts to complete future stages.

  

There are existing implementations of NTT for prime fields that the contestants can study. We want to emphasize that there is already a body of academic work on how to implement NTT efficiently in FPGA as well as optimization targeted for special fields (such as the Polygon Zero’s Goldilocks field or Curve25519 field), and contestants should research extensively before getting started.

  

AMD Xilinx will provide access to the C1100 cards to each competitor for use in the competition. The contestants should discuss with the organizer (see contact information below) on the best way to access the devices.

## Prize Allocation

  

The general idea to distribute the prize is as follows.

-   Every qualified team who passes the first stage and second stage, with codebase that doesn’t seem to be copying from another team, can receive a “performance bonus”. This makes sure that every qualified team is encouraged to continue and finish.
    
-   The speed competition will be awarded according to latency (adjusted by power consumption).
    

  

The final allocation will be released after the team selection.

  

Prizes will be given out in good faith and in the sole discretion of the prize committee.

## Notes

  

All submission code must be open-sourced at the time of submission. Code and documentation must be dual-licensed under both the MIT and Apache-2.0 licenses.

## Questions

  

If there are any questions about this prize, please contact zprize-polygon@dzk.org.
