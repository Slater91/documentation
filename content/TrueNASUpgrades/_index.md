---
title: "Software Releases"
description: "Centralized schedules and upgrade charts for software releases."
weight: 25
related: false
aliases:
 - /scale/gettingstarted/upgrades/
---

## Release List

{{< columns >}}

{{< tabbox name=scale-downloads defaultTab=4 >}}

<--->

{{< tabbox name=core-downloads defaultTab=4 >}}

{{< /columns >}}

Each listed release links to download files for that release.
For the latest deployment and update recommendations from iXsystems, see the [Software Status page](https://www.truenas.com/software-status/).

Bug tickets are typically accepted for the latest release of the current stable version.
Nightly builds also accept feedback and bug tickets.

### Nightly Builds

{{< include file="_includes/NightlyTestWarning.md" >}}

Nightly builds are automatically published when automated testing passes.
**.iso** files are available to fresh install on disposable hardware or a virtual machine.
Switching a disposable system from CORE to SCALE typically requires a fresh install using a nightly .iso file.

**.update** files are also available for manually updating an existing experimental system to a nightly build.

Your testing and feedback is always welcome!
TrueNAS SCALE nightlies have an [option in the top panel](https://www.truenas.com/docs/scale/scaleuireference/toptoolbar/#how-would-you-rate-this-page?) to submit feedback directly to the development team.
Let us know what is working well and what can be improved!

### Legacy Releases

Legacy TrueNAS versions are provided for historical context and upgrade pathways.
They are provided "as-is" and typically do not receive further maintenance releases.
Individual releases are within each major version.

Legacy releases can only be used by downloading the .iso file and freshly installing to the hardware.
See the [Documentation Archive](https://www.truenas.com/docs/archive/) for content related to these releases.

## Upgrade Paths

{{< columns >}}
**TrueNAS SCALE**

{{< mermaid class="mermaid_sizing" >}}
flowchart LR

A["22.02.4 (Angelfish)"] --> C
B["CORE 13.0-U6.1"] --> C
C["22.12.4.2 (Bluefin)"] --> D
D["23.10.1.3 (Cobia)"]
{{< /mermaid >}}

<--->
**TrueNAS SCALE Enterprise**

{{< mermaid class="mermaid_sizing" >}}
flowchart LR
A("Current 22.12 (Bluefin) release") --> B["22.12.4.2 (Bluefin)"] --> C["23.10.1.3 (Cobia)"]
{{< /mermaid >}}

{{< /columns >}}

## Release Schedules

**The release names and dates provided here are tentative and can change at any time.**

Development timelines for [TrueNAS SCALE](#scale-schedule-timeline), [TrueNAS CORE](#core-schedule-timeline), and [TrueCommand](#truecommand-schedule-timeline) are available below.

{{< columns >}}

{{< releaselist name=scale-releases defaultTab=2 >}}

<--->

{{< releaselist name=core-releases defaultTab=2 >}}

<--->

{{< releaselist name=tc-releases defaultTab=2 >}}

{{< /columns >}}

{{< expand "Individual releases within a major version are labeled as Early, Stable, or Maintenance (expand for details)." "v" >}}

{{< truetable >}}
| Type | Status |
|-----------|-------------|
| Early | Public release of a unstable version that is either not feature complete or has more testing cycles planned. Follows an ALPHA, BETA, and RC naming convention. |
| Stable | Public release of a feature complete and internal and community tested major version. Follows a .0 naming convention. |
| Maintenance | Public release with software bugfixes and additional internal and community testing. Follows a .# naming convention, with small-scope maintenance releases ("hotpatches") following a .#.# convention. |
{{< /truetable >}}

{{< /expand >}}

## Timelines

Releases for major versions can overlap while a new major version is working towards a stable release and the previous major version is still receiving maintenance updates.

{{< timeline name="scale-releases" >}}

{{< timeline name="core-releases" >}}

{{< timeline name="tc-releases" >}}
