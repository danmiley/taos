# Phase 2: Geology Deep Dive - Handoff Query for New Agent

## Project Context

**Project**: Taos, New Mexico Regional Concordance  
**Current Status**: Phase 1 (Extended Overview) ✅ **COMPLETE** - All 10 parts finished (~1,300 lines)  
**Next Phase**: Phase 2 - Geology Deep Dive (Significant Geological Features)

---

## What's Been Completed

✅ **Phase 1: Extended Overview** (10 parts, ~1,300 lines)
- Part 1: Basic Information & Geographic Overview
- Part 2: Geological Foundation & Tectonic History
- Part 3: Geography - Topography, Climate, Hydrology
- Part 4: Evolutionary History & Paleontology
- Part 5: Natural History: Flora Overview
- Part 6: Natural History: Fauna Overview
- Part 7: Human History: Prehistory to Colonial
- Part 8: Human History: Modern Era
- Part 9: Cultural Organization & Demographics
- Part 10: Significant Figures, Legacy, Sources

**Key Reference**: Part 2 of the extended overview (`drafts/overview/taos-extended-overview-part-2.md`) contains foundational geological information you can build upon.

---

## Your Task: Phase 2 - Individual Geological Features

### Objective

Create **4-8 individual geological feature documents** for Taos, New Mexico. Each feature should be a standalone document (~200-450 lines) that tells the compelling story of a specific geological formation or feature.

### Scope

| Document Type | Count | Lines Each | Total Lines |
|---------------|-------|------------|-------------|
| Geological Features | 4-8 | ~200-450 | ~800-3,600 |

**Note**: The main geology overview document (`taos-geology.md`) will be created separately. Your focus is on **individual features**.

---

## Feature Selection Criteria

Select features that meet these criteria (prioritize features with multiple criteria):

1. **High Narrative Value**: Features with multiple `[PARADOX]`, `[UNUSUAL]`, `[HUMAN]` flags
2. **Type Localities or Superlatives**: Features that are "the largest," "the oldest," "the only," or type localities
3. **Geology-Human Connections**: Features with climbing history, discovery stories, or indigenous knowledge
4. **Visitor-Accessible**: Features that visitors can see and experience directly

### Potential Features to Consider

Based on Part 2 of the extended overview, consider these features:

1. **Rio Grande Gorge** - 800-foot-deep gorge carved through volcanic basalt; invisible from valley floor `[UNEXPECTED]` `[UNUSUAL]`
2. **Wheeler Peak** - Highest point in New Mexico (13,161 ft); Precambrian basement rocks exposed `[UNUSUAL]`
3. **Taos Plateau Volcanic Field** - Massive basalt flows (5-3 Ma) creating the plateau `[UNUSUAL]`
4. **Sangre de Cristo Fault System** - Active faulting along mountain front `[TURNING]`
5. **Servilleta Basalt Formation** - Primary volcanic flow forming Taos Plateau `[UNUSUAL]`
6. **Rio Grande Gorge Bridge** - Engineering feat spanning the gorge `[HUMAN]`
7. **[Additional features TBD]** - Research may reveal other compelling features

**Your task**: Research and select 4-8 features that best meet the criteria above. You may choose from the list above or discover others through research.

---

## Document Structure

### Template Location
Use: `templates/geological-feature-template.md`

### Required Sections

Each feature document must include:

1. **Overview** (2-3 paragraphs) - Lead with the most compelling hook
2. **Quick Facts Table** - Elevation, dimensions, rock type, age, etc.
3. **Narrative Highlights Table** - Flagged stories (`[PARADOX]`, `[UNUSUAL]`, `[HUMAN]`, etc.)
4. **Deep Time Context** - When rock formed, how exposed, ongoing processes
5. **Formation Process** - Step-by-step explanation
6. **Composition and Structure** - What it's made of
7. **Geology-Human Connections** - Discovery, climbing, indigenous knowledge, tourism
8. **Scientific Significance** - Why geologists study it
9. **Current Status** - Conservation, threats, research
10. **Visitor Information** - How to see/access it
11. **Cross-References** - Links to related documents

### Document Length Guidelines

- **High narrative value** (multiple flags): ~350-450 lines
- **Medium narrative value**: ~250-300 lines
- **Standard features**: ~200-250 lines

**Target**: Aim for 4-8 features totaling ~800-3,600 lines

---

## Narrative Weighting Requirements

**CRITICAL**: Apply narrative weighting throughout. Flag content with:

- `[UNEXPECTED]` - Counter-intuitive facts (e.g., gorge invisible until rim reached)
- `[PARADOX]` - Apparent contradictions explained (e.g., why features exist where they shouldn't)
- `[UNUSUAL]` - Superlatives, rarities, type localities (e.g., highest point in state)
- `[HUMAN]` - Discovery stories, climbers, indigenous knowledge, researchers
- `[TURNING]` - Events that changed understanding, catastrophic events

**Goal**: Make readers say "I never knew that!" while maintaining factual accuracy.

---

## Research Framework

### Query Template Location
Reference: `queries/geological-survey-query.md`

### Key Research Questions

For each feature, research:

1. **Formation Process**: How did this feature form? What geological processes created it?
2. **Deep Time**: When did the rock form? When was it exposed? How has it changed?
3. **Unique Characteristics**: What makes this feature special or unusual?
4. **Discovery History**: Who first documented it? When? What was the story? `[HUMAN]`
5. **Scientific Significance**: Why do geologists study it? What does it reveal?
6. **Human Connections**: Climbing history? Indigenous knowledge? Tourism? Engineering?
7. **Current Status**: Any threats? Conservation status? Ongoing research?

### Sources to Consult

- Part 2 of extended overview (`drafts/overview/taos-extended-overview-part-2.md`)
- Geological surveys and research papers
- Climbing guides and outdoor recreation resources
- Indigenous knowledge and oral histories (if available)
- Visitor information and tourism resources

---

## File Organization

### File Locations

**Create feature documents in**: `/drafts/geology/`

**File Naming Convention**: 
- Use descriptive, lowercase names with hyphens
- Examples: `rio-grande-gorge.md`, `wheeler-peak.md`, `taos-plateau-volcanic-field.md`

### Cross-References

Each feature document should:
- Link to the main geology overview (when created): `[taos-geology.md](taos-geology.md)`
- Link to Part 2 of extended overview: `[taos-extended-overview-part-2.md](../overview/taos-extended-overview-part-2.md)`
- Link to related features (if applicable)

---

## Example Feature Document Structure

```markdown
---
title: "Rio Grande Gorge"
type: geological-feature
region: Taos, New Mexico
date: [YYYY-MM-DD]
tags: [geology, gorge, volcanic, rio-grande]
status: draft
sources: [research, geological-surveys]
related: [taos-geology.md, taos-extended-overview-part-2.md]
narrative_flags: [UNEXPECTED, UNUSUAL, HUMAN, TURNING]
---

# Rio Grande Gorge

## Overview
[Lead with: The gorge is invisible from the valley floor until you reach its rim - 800 feet deep, carved through volcanic basalt...]

## Quick Facts
| Attribute | Value |
|----------|-------|
| **Depth** | Up to 800 feet |
| **Width** | 200-300 feet at river level |
| **Rock Type** | Servilleta Basalt |
| **Age of Rock** | 5-3 million years ago |
| **Age of Landform** | 5 Ma - present (ongoing incision) |

## Narrative Highlights
| Flag | Geological Story |
|------|------------------|
| `[UNEXPECTED]` | Gorge invisible from valley floor until rim reached |
| `[UNUSUAL]` | One of deepest gorges in American Southwest |
| `[HUMAN]` | Rio Grande Gorge Bridge construction story |
| `[TURNING]` | River's persistent downcutting through basalt |

[... continue with all required sections ...]
```

---

## Quality Checklist

Before completing each feature document, verify:

- [ ] All required sections included
- [ ] Narrative weighting applied throughout
- [ ] Flags used for compelling content (`[UNEXPECTED]`, `[PARADOX]`, `[UNUSUAL]`, `[HUMAN]`, `[TURNING]`)
- [ ] Deep Time Context section explains formation, exposure, and ongoing processes
- [ ] Geology-Human Connections section included
- [ ] Sources noted
- [ ] Cross-references to related documents
- [ ] Target length met (200-450 lines based on narrative value)
- [ ] File saved in `/drafts/geology/` with proper naming

---

## Project Files Reference

**Key Files to Review**:
- `PROJECT-STATUS.md` - Overall project status and scope
- `README.md` - Project overview and methodology
- `BOOTSTRAP-QUERIES.md` - Research query templates
- `drafts/overview/taos-extended-overview-part-2.md` - Geological foundation
- `templates/geological-feature-template.md` - Document template
- `queries/geological-survey-query.md` - Research framework

---

## Questions to Answer During Research

1. **Which 4-8 features best meet the selection criteria?**
2. **What makes each feature narratively compelling?**
3. **What are the discovery stories?** `[HUMAN]`
4. **What superlatives or unique characteristics exist?** `[UNUSUAL]`
5. **What paradoxes or counter-intuitive aspects?** `[PARADOX]` `[UNEXPECTED]`
6. **What turning points in understanding?** `[TURNING]`
7. **How do humans interact with each feature?**

---

## Success Criteria

Phase 2 is complete when you have:

- ✅ 4-8 geological feature documents created
- ✅ Each document is 200-450 lines (based on narrative value)
- ✅ Total output: ~800-3,600 lines
- ✅ All documents include required sections
- ✅ Narrative weighting applied throughout
- ✅ Files saved in `/drafts/geology/` with proper naming
- ✅ Cross-references included

---

## Next Steps After Phase 2

After completing Phase 2 features, the project will move to:
- Phase 2.1: Main geology overview document (`taos-geology.md`)
- Phase 3: Geography Documentation
- Phase 4: Evolutionary History (3-document structure)
- Phase 5: Natural History (requires Phase 8 biographies for quotes)
- Phase 6: Human History
- Phase 7: Cultural Organization
- Phase 8: Significant Figures (8 biographies - see PROJECT-STATUS.md)

---

## Getting Started

1. **Review** `drafts/overview/taos-extended-overview-part-2.md` for geological foundation
2. **Review** `templates/geological-feature-template.md` for document structure
3. **Research** potential features and select 4-8 that meet criteria
4. **Create** first feature document following template
5. **Apply** narrative weighting throughout
6. **Repeat** for remaining features

**Good luck! Focus on telling compelling geological stories that make readers say "I never knew that!"**

---

*Handoff Query for Phase 2: Geology Deep Dive - Significant Features*  
*Last Updated: 2025-12-24*


