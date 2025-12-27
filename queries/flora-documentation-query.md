---
title: Flora Documentation Query Template
type: query_template
purpose: Plant species and botanical research framework
date_created: 2025-11-29
status: active
usage: Use to gather flora information for a geographic region
---

# Flora Documentation Query Template

## Purpose

This template provides a structured framework for researching and documenting the plant species and botanical characteristics of a region, with emphasis on endemic species, conservation, and ecological relationships.

## How to Use This Template

1. Use for both overview documentation and individual species profiles
2. Apply narrative weighting—plants have compelling stories
3. Focus on endemic species, conservation struggles, and ethnobotanical connections
4. Note sources for all information
5. Organize findings for flora documentation

---

## Recommended Scope and Structure

Based on successful implementations, flora documentation should include:

### Document Structure

| Document Type | Target Length | Purpose |
|---------------|---------------|---------|
| **Flora Overview** | ~400 lines | Comprehensive vegetation summary |
| **High-Profile Species** | ~350-400 lines | Endemic, flagship, conservation stories |
| **Standard Species** | ~250-300 lines | Ecologically important species |

### Recommended Species Count

- **Minimum**: 1 overview + 4 species profiles (~5 documents)
- **Standard**: 1 overview + 6 species profiles (~7 documents)
- **Comprehensive**: 1 overview + 8-10 species profiles (~9-11 documents)

### Species Selection Criteria

Prioritize species that provide:

| Criterion | Example Species Types |
|-----------|----------------------|
| **Endemic/Regional Specialty** | Found only here or primarily here |
| **Conservation Story** | Threatened, recovering, or extinct species `[TURNING]` |
| **Indigenous Connection** | Species with documented traditional use `[HUMAN]` |
| **Ecological Keystone** | Species that shape ecosystems |
| **Habitat Diversity** | Cover different elevation zones, ecosystems |
| **Climate Indicator** | Species vulnerable to or indicating climate change |
| **Visitor Recognition** | Flagship species visitors expect to see |

### Habitat Coverage Balance

Ensure species selection covers the region's major habitats:

- Different elevation zones (lowland to alpine, if applicable)
- Different ecosystem types (forest, meadow, riparian, etc.)
- Seasonal diversity (spring ephemerals, summer blooms, etc.)

### Biographical Lead Quote Feature

Each species document should open with an **inspiring quote** from a project biographical figure:

| Quote Source Priority | Description |
|----------------------|-------------|
| 1. Direct mention | Quote specifically about the species |
| 2. Habitat reference | Quote about the ecosystem where species lives |
| 3. General nature | Quote about wildness or plant life generally |

Format:
```markdown
> "[Quote text]"
> — **[Figure Name]**, *[Source Title]* ([Year])
```

Research quotes from figures in `/docs/biographies/` before drafting species profiles.

---

## Research Prompt - Overview

```
Research and compile comprehensive flora documentation for [REGION-NAME]:

VEGETATION OVERVIEW
- What are the major plant communities/vegetation types?
- What are the dominant species in each community?
- How is vegetation distributed across the region?
- What are the main vegetation zones (by elevation, moisture, etc.)?
- What seasonal patterns exist?

SPECIES DIVERSITY
- How many plant species are documented?
- What are the major plant families represented?
- How does diversity compare to similar regions?
- What is the ratio of native to non-native species?

ENDEMIC SPECIES
- What plant species are found ONLY in this region?
- How did they evolve/become endemic?
- What are their conservation statuses?
- What makes them unique?
- Where exactly can they be found?

NOTABLE SPECIES
- What are the most ecologically important species?
- What are the most visually striking/recognizable species?
- What species have the most interesting life histories?
- What species have cultural significance?

THREATENED FLORA
- What species are listed as threatened or endangered?
- What are the primary threats to each?
- What conservation efforts are underway?
- What recovery successes have occurred?
- What species have been lost from the region?

INVASIVE SPECIES
- What non-native species are causing problems?
- How did they arrive?
- What damage do they cause?
- What control efforts exist?

ECOLOGICAL RELATIONSHIPS
- What are the key plant-pollinator relationships?
- What plants are critical food sources for fauna?
- What symbiotic relationships exist (mycorrhizae, etc.)?
- How do plants shape the physical environment?

ETHNOBOTANY
- What plants were/are used by indigenous peoples?
- What traditional names exist?
- What medicinal, food, or material uses are documented?
- What spiritual/ceremonial significance do plants have?

BOTANICAL RESEARCH
- What major botanical surveys have been conducted?
- Who were the key botanists who studied this region?
- What botanical discoveries were made here?
- What ongoing research is happening?
```

---

## Research Prompt - Individual Species

```
Research and compile documentation for [SPECIES-NAME] in [REGION-NAME]:

TAXONOMY AND IDENTIFICATION
- Scientific name and authority
- Common names (local, regional, indigenous)
- Family and order
- Subspecies or varieties if applicable
- How to identify (key features)

PHYSICAL DESCRIPTION
- Growth form (tree, shrub, herb, vine, etc.)
- Size range (height, spread)
- Leaves (shape, arrangement, texture)
- Flowers (color, size, structure)
- Fruits/seeds (type, size, dispersal)
- Root system
- Bark/stem characteristics

ECOLOGY
- Preferred habitat
- Elevation range
- Soil preferences
- Moisture requirements
- Light requirements
- Temperature tolerance
- Ecological role

DISTRIBUTION
- Range within the region
- Population status
- Historical vs. current range

LIFE HISTORY
- Lifespan
- Reproductive strategy
- Flowering/fruiting season
- Germination requirements
- Growth rate

CONSERVATION
- IUCN or regional conservation status
- Population trends
- Threats
- Protection efforts
- Success stories

HUMAN CONNECTIONS
- Traditional uses
- Cultural significance
- Discovery history
- Named for whom?

INTERESTING FACTS
- What surprises people about this species?
- What is unique about it?
- What stories are associated with it?
```

---

## Narrative Weighting Focus

For flora documentation, prioritize:

| Criterion | Look For |
|-----------|----------|
| `[UNEXPECTED]` | Plants with surprising characteristics or abilities |
| `[UNUSUAL]` | Endemic species, rare plants, unusual adaptations |
| `[TURNING]` | Conservation battles won or lost, near-extinction recoveries |
| `[HUMAN]` | Ethnobotanical uses, discoverer stories, conservation heroes |
| `[PARADOX]` | Plants that thrive in seemingly impossible conditions |

---

## Key Questions to Answer

### Uniqueness Questions
- What plants exist only here? `[UNUSUAL]`
- What adaptations evolved specifically for this region's conditions?
- What plant surprises botanists? `[UNEXPECTED]`

### Conservation Questions
- What species nearly went extinct but recovered? `[TURNING]`
- What species was lost and what does that teach us?
- What conservation battle is being fought now?

### Human Connection Questions
- What plants were most important to indigenous peoples? `[HUMAN]`
- What discovery story is most interesting? `[HUMAN]`
- What plant has the most unusual human use?

### Ecological Questions
- What plant is the keystone of its ecosystem?
- What plant-animal relationships are critical?
- What plant shapes the landscape most dramatically?

---

## Example Narrative-Weighted Findings

**High Narrative Weight:**
- "The Ghost Orchid was thought extinct for 30 years until a single population was discovered in 2012 by a hiker who had gotten lost." `[TURNING]` `[HUMAN]`
- "This tree produces chemicals so toxic that even standing under it during rain can cause severe burns—yet one moth species depends entirely on it for reproduction." `[PARADOX]` `[UNUSUAL]`
- "Indigenous peoples used the root of this plant to catch fish—it temporarily stuns them without killing them or affecting the meat." `[HUMAN]` `[UNEXPECTED]`
- "Despite appearing completely dead and brown for 11 months of the year, this plant can photosynthesize and produce seeds within 48 hours of the first rain." `[UNUSUAL]`

**Supporting Context:**
- "The region supports approximately 1,500 vascular plant species."
- "Dominant vegetation types include oak woodland, chaparral, and riparian forest."

---

## Output Structure

### Primary Findings (High Narrative Weight)
Compelling plant stories and discoveries:
- [Finding] `[FLAG]` - Source

### Supporting Context (Essential Background)
Standard botanical data:
- [Fact with source]

---

## Narrative Weighting Instructions

Apply these criteria to prioritize content with high narrative value:

1. **The Unexpected** `[UNEXPECTED]` — Surprising plant abilities or characteristics
2. **Paradox Resolution** `[PARADOX]` — Plants thriving in impossible conditions
3. **The Unusual** `[UNUSUAL]` — Endemic species, rare plants, evolutionary oddities
4. **Human Interest** `[HUMAN]` — Ethnobotany, discoverers, conservation heroes
5. **Turning Points** `[TURNING]` — Conservation victories and defeats

### Output Format

**Primary Findings** (high narrative weight):
- [Fact with source] `[CRITERION-FLAG]`

**Supporting Context** (essential background):
- [Background fact with source]

Maintain factual accuracy. Narrative interest guides selection, never overrides truthfulness.

---

*Query template for flora documentation*



