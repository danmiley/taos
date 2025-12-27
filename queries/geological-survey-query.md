---
title: Geological Survey Query Template
type: query_template
purpose: Comprehensive geological research framework with multi-document structure
date_created: 2025-11-29
date_updated: 2025-11-30
status: active
usage: Use to gather geological information and create multi-document geology section
---

# Geological Survey Query Template

## Purpose

This template provides a structured framework for researching and compiling comprehensive geological documentation of a region. It guides creation of a **multi-document structure**: one main overview plus individual feature documents.

## Document Structure and Length Guidelines

| Document Type | Target Length | Content Focus | Narrative Density |
|---------------|---------------|---------------|-------------------|
| **Main Overview** (`[region]-geology.md`) | ~500-550 lines | Comprehensive regional geology | High |
| **High-Value Feature** (`[feature].md`) | ~350-450 lines | Major feature with rich narrative | Very High |
| **Standard Feature** (`[feature].md`) | ~250-300 lines | Notable feature with clear story | Medium-High |
| **Brief Feature** (`[feature].md`) | ~200-250 lines | Feature with focused narrative | Medium |

## How to Use This Template

1. **Research main overview content** using Section 1 prompts
2. **Identify notable features** (4-8 recommended) for individual documents
3. **Assess narrative value** of each feature to determine length
4. **Research each feature** using Section 2 prompts
5. **Apply narrative weighting** throughout
6. **Note sources** for all information
7. **Complete checklists** before finalizing

---

## Section 1: Main Overview Research

### Research Prompt for Main Overview

```
Research and compile comprehensive geological documentation for [REGION-NAME]:

TECTONIC SETTING
- What tectonic plate(s) is the region on?
- What type of plate boundary (if any) affects it?
- What geological province does it belong to?
- What is the tectonic history over geological time?
- What ongoing tectonic processes are occurring?

GEOLOGICAL TIMELINE
For each major era (Precambrian, Paleozoic, Mesozoic, Cenozoic):
- What rocks and formations date from this period?
- What environments existed during this time?
- What major geological events occurred?
- What evidence remains visible today?

ROCK TYPES AND NAMED FORMATIONS
- What distinct plutons or formations exist? (Names, ages, compositions)
- What makes each formation distinctive?
- Are any formations "type localities" (where rock type was first described)?
- How do different rock types affect landscape and features?

GEOLOGICAL HAZARDS
- What seismic activity occurs (fault systems, earthquake history)?
- What mass wasting risks exist (rockfall, landslides)?
- What are specific major events with dates?
- What ongoing monitoring exists?

RESEARCH HISTORY
- Who were the key geologists who studied this region?
- What major geological debates occurred here?
- What discoveries changed scientific understanding?
- What ongoing research is happening?
```

### Main Overview Required Sections

| Section | Content | Narrative Focus |
|---------|---------|-----------------|
| Narrative Highlights | Table of key stories with flags | All flags |
| Tectonic Setting | Plate context; current activity | `[TURNING]` events |
| Geological Timeline | Era-by-era with regional specifics | `[UNEXPECTED]` deep time facts |
| Rock Types | Named formations with characteristics | `[UNUSUAL]` type localities |
| Geological Hazards | Specific events; ongoing risks | `[TURNING]` disasters |
| Notable Features | Summary table linking to feature docs | All flags |
| Research History | Key figures and discoveries | `[HUMAN]` scientists |

---

## Section 2: Feature Document Research

### Feature Selection Criteria

Select 4-8 features for individual documentation based on:

| Criterion | Question | Ideal Answer |
|-----------|----------|--------------|
| **Narrative richness** | Does it have a compelling story or paradox? | Yes—multiple angles |
| **Superlative status** | Is it largest, oldest, first, or only? | Yes—documentable claim |
| **Human connection** | Does geology connect to human activity? | Yes—climbing, discovery, use |
| **Visitor experience** | Can visitors see and experience the geology? | Yes—accessible evidence |
| **Scientific significance** | Is it a type locality or study site? | Yes—named for this place |

### Assess Narrative Value

For each potential feature, score these criteria:

| Criterion | Low (1) | Medium (2) | High (3) |
|-----------|---------|------------|----------|
| **Paradox potential** | No counter-intuitive aspects | Minor paradox | Major paradox that surprises |
| **Human story** | No significant human connection | Some history | Rich discovery/use story |
| **Visual drama** | Subtle feature | Notable feature | Iconic/dramatic feature |
| **Scientific significance** | Common type | Regional importance | Type locality or global significance |
| **Visitor relevance** | Hard to access | Visible but distant | Can experience directly |

**Scoring guide**:
- 12-15 points: Very High value → ~350-450 lines
- 9-11 points: High value → ~250-350 lines
- 5-8 points: Medium value → ~200-250 lines

### Research Prompt for Each Feature

```
Research [FEATURE-NAME] in [REGION-NAME] for geological documentation:

BASIC FACTS
- What type of feature is it? (dome, cliff, waterfall, canyon, etc.)
- What are its dimensions/measurements?
- What rock type(s) compose it?
- How old is the rock? How old is the current landform?

DEEP TIME CONTEXT
- When did the rock crystallize/deposit? Under what conditions?
- How was it exposed? (erosion, uplift, glaciation?)
- How was it shaped into current form? (weathering, glacial carving, exfoliation?)
- What ongoing processes continue to modify it?
- How will it change in the geological future?

FORMATION PROCESS
- What process created this feature? Explain step by step.
- Are there counter-intuitive aspects to the formation? `[PARADOX]`
- How does this feature compare to similar features elsewhere?

HUMAN CONNECTIONS
- Who first documented or studied this feature? When? `[HUMAN]`
- What indigenous names exist? What do they reveal about the feature?
- How do climbers, visitors, or researchers interact with the geology?
- Does geological knowledge enable human activities here?

SUPERLATIVES AND SIGNIFICANCE
- Is this feature a superlative (largest, oldest, only, first)? `[UNUSUAL]`
- Is it a type locality for any rock or formation? `[UNUSUAL]`
- What makes it scientifically significant?

VIEWING AND ACCESS
- Where can visitors see this feature?
- What geological evidence is visible?
- What's the best way to understand the geology?
```

### Feature Document Required Sections

| Section | Content | Notes |
|---------|---------|-------|
| Overview | 2-3 paragraphs introducing the feature | Lead with the hook |
| Quick Facts | Table of key measurements and data | Standardized format |
| Narrative Highlights | Table of stories with flags | 3-5 key narratives |
| Deep Time Context | When formed → how exposed → current processes | Always include |
| Formation Process | Step-by-step explanation | Make accessible |
| [Process Name] Section | Detailed explanation if relevant (e.g., "Exfoliation") | For key processes |
| Human Connections | Discovery, naming, use | Required where applicable |
| Viewing and Access | Where to see; what to look for | Practical information |
| Cross-References | Links to related documents | Maintain connections |

---

## Section 3: Geological Process Explanations

### Common Processes to Document

For regions with these processes, create explanatory sections:

| Process | Counter-Intuitive Aspect | Flag |
|---------|-------------------------|------|
| **Exfoliation** | Domes form from expansion, not compression | `[PARADOX]` |
| **Glacial Carving** | Hanging valleys from differential erosion | `[PARADOX]` |
| **Pluton Formation** | Rock crystallized miles underground | `[UNEXPECTED]` |
| **Uplift/Exposure** | Deep rock now at surface after millions of years | `[UNEXPECTED]` |
| **Rockfall** | Landscape still actively changing | `[TURNING]` |

### Exfoliation Explanation Template

```
How Exfoliation Works:

1. DEEP BURIAL
   - Rock crystallizes miles underground under immense pressure
   - Granite is compressed in all directions

2. SLOW UNROOFING  
   - Erosion removes overlying rock over millions of years
   - Pressure gradually decreases

3. EXPANSION BEGINS
   - Released from pressure, surface rock expands
   - Interior rock still confined—expands less

4. FRACTURES DEVELOP
   - Differential expansion creates stress
   - Fractures form parallel to surface
   - Concentric shells develop (like onion layers)

5. WEATHERING REMOVES SHELLS
   - Water enters fractures, freezes, expands
   - Root growth pries shells loose
   - Gravity removes loosened material
   - Rounded dome shape develops

THE PARADOX: Domes form from EXPANSION, not compression—counter-intuitive!
```

### Hanging Valley Explanation Template

```
How Hanging Valleys Form:

1. PRE-GLACIAL LANDSCAPE
   - Main river and tributaries flow at matching grades
   - No waterfalls—streams descend gradually

2. GLACIATION BEGINS
   - Ice accumulates in valleys
   - Glaciers form in main valley and tributaries

3. DIFFERENTIAL EROSION
   - Main valley glacier is larger—erodes faster
   - Tributary glacier is smaller—erodes slower
   - Main valley floor drops relative to tributary

4. ICE MELTS
   - Tributary floor now "hangs" above main valley
   - Stream drops over cliff as waterfall

THE PARADOX: Waterfall height reflects glacier SIZE difference, not stream size!
```

---

## Section 4: Narrative Weighting for Geology

### Prioritize Content With High Narrative Value

| Flag | What to Look For in Geology |
|------|----------------------------|
| `[PARADOX]` | Counter-intuitive processes (expansion creates domes); features that look like something else (Half Dome's "missing half" was never there); absence that IS the story |
| `[UNUSUAL]` | Superlatives (largest, tallest, oldest); type localities; unique rock types; rare formations |
| `[UNEXPECTED]` | Geology enabling human activity (climbing routes follow geological features); ancient rock in unexpected places; processes still happening |
| `[TURNING]` | Views that proved theories; catastrophic events with specific dates; discoveries that changed understanding |
| `[HUMAN]` | Scientists who made discoveries; debates (Whitney vs. Muir); climbers using geological knowledge; indigenous understanding |

### Example High-Narrative Geological Content

**Very High Narrative Weight:**
- "The dome never had another half—the name enshrines a geological misunderstanding. The sheer face formed by exfoliation along vertical joints, not from breaking." `[PARADOX]`
- "This is the largest exposed granite monolith on Earth—3,000 vertical feet of continuous rock without a major ledge." `[UNUSUAL]`
- "Alex Honnold's free solo was enabled by geology: the continuous face with minimal jointing meant he could plan every move." `[HUMAN]` `[UNEXPECTED]`

**High Narrative Weight:**
- "State Geologist Whitney said the valley floor 'dropped'; self-taught John Muir proved glaciers carved it. The view from this point made Muir's case undeniable." `[TURNING]` `[HUMAN]`
- "The Ahwahneechee called it 'Spirit of the Puffing Wind'—they understood that the valley's geometry creates actual updrafts that deflect the waterfall." `[HUMAN]` `[UNEXPECTED]`

**Supporting Context (Essential but lower narrative weight):**
- "The granite crystallized approximately 95-100 million years ago at depths of 6-10 miles."
- "The region experiences approximately 50 measurable seismic events annually."

---

## Section 5: Checklists

### Main Overview Checklist

- [ ] Narrative Highlights table with 4-6 flagged stories
- [ ] Tectonic setting with current activity
- [ ] Geological timeline (era by era)
- [ ] Named rock formations with ages and characteristics
- [ ] At least one `[PARADOX]` explained
- [ ] Major geological debate documented `[HUMAN]`
- [ ] Notable features summary table with links
- [ ] Research history with key figures
- [ ] Sources cited

### Feature Document Checklist

- [ ] Quick Facts table complete
- [ ] Narrative Highlights table with 3-5 flags
- [ ] Deep Time Context section (formation → exposure → ongoing)
- [ ] Formation process explained accessibly
- [ ] Counter-intuitive aspects flagged `[PARADOX]`
- [ ] Human connections documented
- [ ] Superlative status noted if applicable `[UNUSUAL]`
- [ ] Viewing/access information included
- [ ] Cross-references to related features
- [ ] Sources cited

---

## Output Format

### Primary Findings (High Narrative Weight)

```markdown
## [Feature/Topic]

**Narrative Highlights:**
| Flag | Story |
|------|-------|
| `[PARADOX]` | [Counter-intuitive fact] |
| `[HUMAN]` | [Discovery or use story] |

[Finding with explanation] `[FLAG]` — Source
```

### Supporting Context (Essential Background)

```markdown
### Technical Details
- [Fact with source]
- [Measurement with source]
```

---

## Example Feature Assessment

### Feature: [Example Peak]

**Narrative Value Assessment:**
| Criterion | Score | Notes |
|-----------|-------|-------|
| Paradox potential | 3 | Name implies something false |
| Human story | 3 | Rich climbing history; discovery story |
| Visual drama | 3 | Iconic landmark |
| Scientific significance | 2 | Regional importance |
| Visitor relevance | 3 | Highly accessible |
| **Total** | **14** | **Very High → ~400 lines** |

**Key Narratives Identified:**
1. `[PARADOX]` - The "missing" part was never there
2. `[HUMAN]` - First ascent story and method
3. `[UNEXPECTED]` - Formation process (expansion not compression)
4. `[TURNING]` - Evidence still visible of ongoing process

---

*Query template for comprehensive geological research and multi-document creation*
*Updated: 2025-11-30*


