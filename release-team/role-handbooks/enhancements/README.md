# Enhancements Lead Handbook

## Overview

While the Enhancements Lead serves as a member of the Release Team (a subproject of [SIG Release][sig-release]), this role is also a liaison to [SIG PM][sig-pm] across the following subprojects:
- Product Management
- Program Management & Release
- Release Marketing

## Responsibilities

An Enhancements Lead holds the following responsibilities:
- Maintain the active status of Enhancements within [kubernetes/enhancements][k/enhancements]
- Facilitate communication between Enhancement Owners, Product Management, and SIG leadership, as necessary
- Collate the major themes of the release, including but not limited to:
  - new enhancements
  - long-awaited enhancements
  - enhancements moving into GA
  - enhancement deprecations
  - notable changes to existing behaviors
- Assist in Communications activities (in conjunction with the Communications Lead & the CNCF Communications team):
  - Draft and / or review https://kubernetes.io/blog/ release announcement post, leveraging the themes collected across the release cycle e.g., [1.11 Announcement][1.11-announcement]
  - Engage with media analysts during the embargo period to discuss the release themes
  - CNCF Kubernetes Release webinar
  - Identify potential contributors for the “5 Days of Kubernetes” blog series
  - Identify candidates to assume the Enhancements Lead role (according to the [Release Team selection process][rt-selection]) in the following release cycle

## General Requirements

In addition to the [requirements detailed for all Release Team members][rt-requirements], becoming an Enhancements Lead has additional gates:
  - MUST have served on the Release Team in a previous capacity, ideally as an Enhancements Shadow
  - MUST be a member of the [SIG Release Google Group][sig-release-group]
  - MUST be a member of the [SIG PM Google Group][sig-pm-group]
  - MUST be a member of the [Kubernetes Milestone Burndown Google Group][burndown-group]

Helpful characteristics of an Enhancements Lead include:
- experience with the Kubernetes community, code layout, ecosystem projects, organizational norms, governance, SIG structure, architecture, and release process
- product / project / program management experience
- release management experience

## Mentoring Shadows

## Getting Started

### Access Required
Ensure that the previous Enhancements Lead has given (or facilitated getting) you access to:
- GitHub teams
  - enhancements-maintainers
  - kubernetes-milestone-maintainers
- OWNERS_ALIASES (as `enhancements-maintainers` in [kubernetes/enhancements][k/enhancements] repo)
- Edit access to the Kubernetes x.y.0 Enhancements Tracking Sheet e.g., [Kubernetes 1.12 Enhancements Tracking][1.12-tracking]

## Process

### Standards
As mentioned previously, the Enhancements Lead role encompasses several cross-functional responsibilities with [SIG PM][sig-pm].

The process of maintaining an enhancement in Kubernetes is documented in the [kubernetes/enhancements][k/enhancements] repo. Any questions / concerns / suggestions for improvement to the Enhancements process should be raised as GitHub issues / PRs to k/enhancements.

It is important that this process be followed and documentation remain up-to-date as the [Enhancements repo][k/enhancements] is the primary ingress point for contributors interested in tracking enhancements.

### Milestone Activities + Timing
- Link items from succession section
- (optional) Watch the kubernetes/enhancements repo to get notified on all issues
- Ensure that Enhancement Tracking sheet for the new release was created by the previous Enhancements Lead and populated with the enhancements removed from the previous milestone
- Enhancements Tracking sheet is shortlinked with the pattern `k8sxyy-enhancements` e.g., http://bit.ly/k8s113-enhancements
- Ensure the Enhancements Tracking sheet has the appropriate permissions:
ownership transferred to you
  - anyone who has the link can comment
  - Edit access
    - [SIG PM][sig-pm] Chairs
    - [Kubernetes Release Team Google Group][rt-group]
  - Comment access
    - [SIG Release Google Group][sig-release-group]
    - [SIG PM Google Group][sig-pm-group]
    - [SIG Docs Google Group][sig-docs-group]
    - [SIG Leads Google Group][sig-leads-group]
- Work with outgoing Enhancements Lead to elicit information from SIGs on enhancements removed from previous milestone
- Enhancements Triage
  - Check enhancements and ensure they provide the required information and labels to be accepted into the milestone.
    - Enhancements marked for current milestone
    - Enhancements marked for previous milestone
    - Enhancements marked with `next-milestone` (https://github.com/kubernetes/enhancements/issues?q=is%3Aopen+is%3Aissue+milestone%3Anext-milestone+sort%3Acreated-desc)
    - Enhancements without a milestone (https://github.com/kubernetes/enhancements/issues?q=is%3Aopen+is%3Aissue+sort%3Acreated-desc+no%3Amilestone)
    - Enhancements from two or more milestones ago
  - Confirm with the Enhancement Owner if work is planned for current milestone
    - Apply the current milestone
    - Add the enhancement to the Enhancements Tracking sheet
    - Apply the `tracked/yes` label
    - Remove `lifecycle/frozen` label from all issues
- Sync with Product Management Chair (bi-weekly?)

### Escalation / Handling Unresponsive Enhancement Owners
List of unresponsive issues? Add unresponsive status to enhancements tracking?

### Exceptions

### CNCF / Media Engagement

### Succession
- Generate new Enhancements Tracking sheet with enhancements that were removed from the current milestone
- Enhancements Tracking sheet is shortlinked with the pattern `k8sxyy-enhancements` e.g., http://bit.ly/k8s113-enhancements
- Continually work to improve Enhancements process
- Review / update documentation as the release cycle
- Close issues marked as stable that made it into the release
- Close milestones that are complete
- Cleanup old milestones

### Limitations
- Populating the Enhancements Tracking sheet is a manual process
- Enhancements issues that are not submitted to [k/enhancements][k/enhancements] are not actively tracked in the context of the Release Team and Release cycle e.g.,
  - `kubeadm` (https://github.com/kubernetes/kubeadm/issues?utf8=%E2%9C%93&q=is%3Aissue+label%3Akind%2Ffeature+milestone%3Av1.12+)
  - out-of-tree Cloud Provider code that may live in `kubernetes-sigs/*`
  - additional out-of-tree code that may live in the following organizations:
    - `kubernetes`
		- `kubernetes-client`
		- `kubernetes-csi`
		- `kubernetes-incubator`
		- `kubernetes-sig-testing`
		- `kubernetes-sigs`
- Finding consensus on how frequently to triage enhancements

## Signals

## Tips & Tricks

#### Sample Searches (examples)

#### GitHub Notifications
https://groups.google.com/forum/#!topic/kubernetes-dev/5qU8irU7_tE


[burndown-group]: https://groups.google.com/forum/#!forum/kubernetes-milestone-burndown
[k/enhancements]: https://github.com/kubernetes/enhancements
[rt-group]: https://groups.google.com/forum/#!forum/kubernetes-release-team
[rt-selection]: /README.md#release-team-selection
[rt-requirements]: /README.md#release-team-requirements
[sig-docs-group]: https://groups.google.com/forum/#!forum/kubernetes-sig-docs
[sig-leads-group]: https://groups.google.com/forum/#!forum/kubernetes-sig-leads
[sig-pm]: https://github.com/kubernetes/community/blob/master/sig-pm/README.md
[sig-pm-group]: https://groups.google.com/forum/#!forum/kubernetes-pm
[sig-release]: https://github.com/kubernetes/community/blob/master/sig-release/README.md
[sig-release-group]: https://groups.google.com/forum/#!forum/kubernetes-sig-release
[1.11-announcement]: https://kubernetes.io/blog/2018/06/27/kubernetes-1.11-release-announcement/
[1.12-tracking]: http://bit.ly/k8s112-enhancements
