# unity-semantic-asset-merge

> **Working title**
>
> Exploratory Unity editor tool for structure-aware comparison and merging of Unity assets and Scene hierarchies.

---

## Motivation: Why this exists

Merging and comparing Unity Scenes and assets is fragile and stressful — even for solo developers, and especially for teams.

Most existing workflows treat Unity assets as serialized text. This makes it difficult to:

* Understand *what actually changed*
* Safely merge only parts of a Scene, Prefab, or ScriptableObject asset
* Reason about structural changes rather than serialization artifacts
* See the actual outcome in the familiar editor during the merge process

This repository exists to support the development of an in-progress Unity editor tool that approaches Scene and asset merging at a **semantic / structural level**, rather than through raw text-based merges.

---

## What I’m exploring

At a high level, I am looking at ideas such as:

* Comparing and merging
  * GameObject hierarchies
    * Scenes
    * Prefabs
    * Sub-hierarchies within the same Scene
  * ScriptableObjects
* Making conflicts **explicit and inspectable**, instead of auto-resolving everything
* Wizard-like walkthrough of the merge process
* Separating meaningful changes from serialization noise

---

## Who this is for

* Teams struggling with Scene or Prefab merge conflicts
* Developers working in parallel on shared Scenes and Prefabs
* Solo developers who are branching their work or simply want to compare and move data between Unity Objects
* Anyone who wants to inspect a Scene change

---

## What this is not

* Not a finished product
* Not an open-source project
* Not affiliated with Unity Technologies
* Not a promise of features, timelines, or availability

---

This is an early exploration and learning space.

This is a place to learn about updates of development progress.

---

## Current status

* Actively prototyping:
  * **Working model** that generates a **set of changes** between two Scenes, producing an identical Scene upon applying changes in any order.
    * Including Prefab identities and overrides
  * Automatic analysis of **Component constraints** (eg. Components requiring other Components)
  * Early UI and workflow experiments.
  * Conflict and dependency detection.
* Growing set of unit tests to catch all discovered edge cases.

---

## Possible direction

The intent is to eventually turn this into a usable Unity editor tool.

If that happens, this repository will be used to share progress and announcements. Watching the repository is the best way to stay informed.

---

## Join the discussion

Real-world workflows, edge cases, and failure stories are the most valuable input right now.

Anyone who wants to share their experience and workflow with Scene merging, or their approach to avoid Scene conflicts in the first place.
Feel free to share experiences, pain points, and ideas in the **Discussions** tab. Feel free to start a new thread — no need to ask first.

---

## Status & license

This repository currently contains **no source code** and is shared for discussion purposes only.
No license is granted for reuse or redistribution.

---

## About the author

I’m a seasoned Unity developer with 15+ years of professional experience, always trying to improve the workflow.