## Preamble

    EIP: 3
    Title: Funding protocols
    Author: Jordan Brooks <jordan@hyperbridge.org>
    Type: Standard Track
    Category: Core
    Status: Draft
    Created: 2018-05-03

## Simple Summary

A standard for decentralized funding of developer projects on Blockhub.

## Abstract

Smart contracts on a decentralized blockchain facilitating the funding of game developer projects within the Blockhub ecosystem. A standardized protocol for developers to propose project ideas, specify funding requirements, schedule milestones, and outline contribution tiers/incentives. In addition, these protocols would standardize the process for Blockhub users to contribute cryptocurrency to the projects they support, and provide them a platform to vote on the success of individual milestones.

## Specification

### Projects

Game developers can create project proposals to notify Blockhub users of their ideas and acquire funding. These proposals will necessarily include the following information:

* A **title** and accurate **description** of the overall goals of the project.
* **Media** (picture and/or video) and information outlining specific features of the project.
* The **contribution tiers** that Blockhub users who provide cryptocurrency support will fall within. Each tier will outline the minimum and maximum contribution amount, the maximum number of contributors (if applicable), and the rewards/incentives included with a contribution at that tier-level.
* A proposed **timeline** for project development. A single timeline will be composed of multiple **milestones**. Each milestone is associated with a particular percentage of the total funding, released only upon successful completion of the previous milestone (as determined by the contributors of the project). The criteria for completion of a milestone will need to be clearly communicated at the project proposal stage.

### Contributors

Blockhub users can review project proposals and contribute cryptocurrency to projects that they support; in doing so, they are considered "contributors" of that particular project. As a contributor, they are entitled to rewards/incentives, as outlined in their particular contribution tier, at the successful completion of the project. Furthermore, contributors are given a platform to voice their opinion with regards to mileston completion. When a developer completes a milestone, all contributors are notified and must approve/disapprove the current progress. The result of this approval/disapproval process determines the release of subsequent funding from the project contract to the developer. In the case of one or more failed milestones, this may open the door to a refunding of the project.

### API Proposal

#### Developer
   *Instance Variables:*
   
    projects

   *Functions:*
   
    addProject()
    removeProject()
    
#### Project
   *Instance Variables:*
   
    title
    description
    videoLink
    about
    tiers
    contributors
    timeline
    timelineHistory

   *Functions:*
   
    proposeTimelineUpdate()
    finalize()

#### ProjectTier
   *Instance Variables:*
   
    title
    description
    contributors
    rewards
    minContributionAmount
    maxContributionAmount
    currentContributorCount

#### ProjectTimeline
   *Instance Variables:*
   
    milestones
    
   *Functions:*
   
    addMilestone()
    removeMilestone()

#### ProjectMilestone
   *Instance Variables:*
   
    title
    description
    conditions
    isComplete
    
   *Functions:*
   
    complete()

## Rationale

The use of a decentralized funding protocol allows Blockhub to mitigate, or altogether avoid, common issues associated with similar crowdfunding platforms. Specifically, by delegating control of fund allocation to blockchain-based smart contracts, the risk of contributors losing money due to non-viable projects that never reach completion, or due to malicious developers with no intention of project completion, is reduced significantly.

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
