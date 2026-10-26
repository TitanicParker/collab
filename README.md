# Structuracy · Collab

**The public architecture of the Portable Structuracy Corpus.**  
[Open the site source](./index.html) · [The 54 canonical reference](https://github.com/TitanicParker/fiche-ceathar/blob/main/THE_54_CONTROL.md)

This repository documents the procedure by which a sentence's **meaning**, its **structural reading**, and the **recovery of its completed intelligibility** are kept distinct. It is also the future presentation site for approved, navigable sentence cards.

**This repository is not the live blind-solving workspace.** Publishing earlier solved material here does not make it safe to provide this site to a new decoder GPT. The decoder must receive only its restricted input and its own instructions in a fresh context.

## The corpus

The planned domains include 100 literary sentences, 100 scientific sentences, 27 fairy tales with selected sentence-level units, and approximately 590-plus mathematical theorem statements or steps. The final total and the scope of the proposed larger card atlas should be confirmed from the numbered master corpus rather than assumed from rough counts.

The next planned decoding batch is **the first 1,400 completed structural readings**, as supplied by the independent structural-reading process. This README makes no claim that those second-stage resolutions have been completed.

## Document sequence

| Document | Contents | Visibility and purpose |
|---|---|---|
| **0. Master corpus** | Numbered original sentences, source domain and provenance | Protected source |
| **1. Reading archive** | Original sentence, meaningful account, frozen structural reading | Protected complete record |
| **2. Clean handoff** | Verbatim frozen structural reading alone for interpretation | Restricted to decoder GPT; ordinal linkage is external |
| **3. Decoder result** | Candidate three-axis coordinate, strongest rival, rationale, confidence or abstention | Frozen before canonical lookup |
| **4. Approved publication** | Reassembled sentence, meaning, structural reading, recovery account, coordinate, cell number, canonical short form, status and provenance | Public cards only when approved |

## Procedure 1 — Structural reading

A separate GPT examines the original sentence under the structural-reading JSON instrument. It respects what the sentence means, but also describes what the sentence **does**: the participants, relational loci, work of those relations, whole-sentence achievement and interpretive boundary.

The resulting paragraph is frozen. It must not be rewritten to make it resemble a known cell.

### Firewall 1 — Evidence isolation

**Boundary:** Document 1 → Document 2.

The handoff worker extracts the structural-reading field **verbatim**, retaining its complete words and punctuation. The separate original sentence and meaningful reading are excluded. Quoted fragments already embedded in the frozen structural reading remain part of that reading. The ordinal index stays in the coordinator's mapping but need not enter the decoder's prompt.

**Purpose:** The next GPT must not repair gaps in the reading by consulting the original text. The experiment tests whether the structural reading contains enough information for the structural form to be recovered.

**Implementation rule:** A fresh GPT context receives only one structural reading and the decoder procedure. Merely telling a GPT to disregard text it already saw is not a firewall. If a batch format is used, independently assessed items must not inherit prior answers or reveal a growing atlas of resolutions.

## Procedure 2 — Reading-only structural resolution

The second JSON instrument is a **procedure specification** for a separate interpretive GPT, not a deterministic classifier by itself.

Input: **one frozen structural reading only**. The decoder may be given the 15 primitive definitions but neither the original sentence nor the lookup atlas, prior solved examples, preselected cell names or expected answer.

It resolves the unified conjunction:

- **Transformation Pattern (6):** Differentiation, Opening, Relating, Repair, Integration, Settlement.
- **Completion Topology (3):** Focal, Distributed, Release.
- **Persistence Mode (3):** Standing, Bearing, Efficacy.

The decoder identifies its candidate conjunction, explains the evidence, challenges the strongest neighboring rival, and either resolves, marks a provisional candidate, or abstains when evidence is insufficient. It must distinguish the **event described** from the **linguistic achievement** and the **reader's act of understanding**.

### Firewall 2 — Classification freeze

**Boundary:** Document 3 → canonical lookup.

The decoder's coordinate and competing explanation are frozen **before** the authoritative 54-cell names, example atlas or companion utterances become visible.

**Purpose:** Prevent recognition of a familiar canonical example from replacing structural reasoning, and prevent retroactive adjustment of the three axes.

After freezing, the coordinator can apply the zero-based indexing formula `cell = 9 × T + 3 × K + P + 1` or consult the authoritative Fiche Ceathar table. The resulting number and canonical name are **lookup outputs**, not further interpretive decisions.

## Publication and cards

The site at [index.html](./index.html) is a prototype of the eventual swipeable, tap-to-flip atlas, following the interaction language of [The 54 Quiet Flip Deck](https://github.com/TitanicParker/fiche-ceathar/blob/main/the_54_quiet_flip_deck.html) and [Recognition Deck](https://github.com/TitanicParker/fiche-ceathar/blob/main/the_54_recognition_deck_revised.html).

An approved card is designed to hold:

1. Ordinal number, source domain and provenance.
2. Exact original sentence.
3. Meaningful reading.
4. Frozen structural reading.
5. Independent structural-recovery reasoning, candidate three axes and strongest rival.
6. Canonical cell number and short form **only if warranted**, with the resolution status.

Categories support browsing by source domain and, after validation, the three structural dimensions and the 54 cells. Cards should flip on tap, move on swipe and keyboard input, and scale through a reusable interface populated from approved data rather than thousands of handwritten HTML files.

**Publication is downstream of the firewalls.** The GitHub site may display everything already solved and approved, but it must not be used as contextual source material for a fresh decoding GPT. Publicly available answers can contaminate a later decoding experiment if the model is deliberately exposed to them.

## Current state

- Workflow architecture and two explicit firewalls are documented.
- A public-facing `index.html` with a responsive, illustrative card interface has been added.
- Demonstration cards are **not** claims of experimental classification.
- The first 1,400 reading-only second-stage resolutions have **not** been performed by this repository.
- No live corpus records or canonical resolutions are published here yet.

## The experiment's question

Can independently produced structural readings, stripped of their original sentences and meaningful explanations, preserve sufficient evidence for a separate decoder to recover stable, discriminable forms of completed intelligibility across literature, science, fairy tales and mathematics?

The 54 is a candidate grammar to be tested—not a result to be presumed.
