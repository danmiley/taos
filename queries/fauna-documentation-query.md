---
title: Fauna Documentation Query Template
type: query_template
purpose: Animal species and wildlife research framework
date_created: 2025-11-29
status: active
usage: Use to gather fauna information for a geographic region
---

# Fauna Documentation Query Template

## Purpose

This template provides a structured framework for researching and documenting the animal species and wildlife characteristics of a region, with emphasis on endemic species, conservation, and ecological relationships.

## How to Use This Template

1. Use for both overview documentation and individual species profiles
2. Apply narrative weighting—wildlife has dramatic stories
3. Focus on endemic species, conservation struggles, and behavioral oddities
4. Note sources for all information
5. Organize findings for fauna documentation

---

## Recommended Scope and Structure

Based on successful implementations, fauna documentation should include:

### Document Structure

| Document Type | Target Length | Purpose |
|---------------|---------------|---------|
| **Fauna Overview** | ~400 lines | Comprehensive wildlife summary |
| **High-Profile Species** | ~350-400 lines | Endemic, flagship, conservation stories |
| **Standard Species** | ~250-300 lines | Ecologically important species |

### Recommended Species Count

- **Minimum**: 1 overview + 5 species profiles (~6 documents)
- **Standard**: 1 overview + 8 species profiles (~9 documents)
- **Comprehensive**: 1 overview + 10-12 species profiles (~11-13 documents)

### Species Selection Criteria

Prioritize species that provide:

| Criterion | Example Species Types |
|-----------|----------------------|
| **Endemic/Regional Specialty** | Found only here or subspecies unique to region |
| **Conservation Story** | Recovery success, ongoing threats, historical extinction `[TURNING]` |
| **Indigenous Connection** | Species with documented cultural significance `[HUMAN]` |
| **Ecological Keystone** | Predators, herbivores, seed dispersers shaping ecosystems |
| **Habitat Diversity** | Cover terrestrial, aquatic, aerial; different elevations |
| **Climate Sentinel** | Species indicating environmental change |
| **Human-Wildlife Interface** | Species with notable human interactions |
| **Charismatic Megafauna** | Flagship species visitors expect to see |

### Taxonomic Coverage Balance

Ensure species selection covers major groups present in the region:

| Group | Target | Notes |
|-------|--------|-------|
| **Mammals** | 3-5 species | Include predator(s), herbivore(s), small mammal(s) |
| **Birds** | 2-4 species | Include raptor, songbird, or specialty species |
| **Reptiles/Amphibians** | 1-2 species | If regionally significant |
| **Fish** | 1-2 species | Native aquatic species if applicable |
| **Invertebrates** | 0-2 species | Only if regionally iconic or endemic |

### Habitat Coverage Balance

Ensure species selection covers the region's major habitats:

- Different elevation zones (lowland to alpine, if applicable)
- Terrestrial habitats (forest, meadow, rocky areas, etc.)
- Aquatic habitats (rivers, lakes, marine if coastal)
- Aerial species (birds, bats)

### Biographical Lead Quote Feature

Each species document should open with an **inspiring quote** from a project biographical figure:

| Quote Source Priority | Description |
|----------------------|-------------|
| 1. Direct mention | Quote specifically about the species |
| 2. Related species | Quote about similar or related animals |
| 3. Habitat reference | Quote about the ecosystem where species lives |
| 4. General wildlife | Quote about animals or wildness generally |

Format:
```markdown
> "[Quote text]"
> — **[Figure Name]**, *[Source Title]* ([Year])
```

Research quotes from figures in `/docs/biographies/` before drafting species profiles.

---

## Research Prompt - Overview

```
Research and compile comprehensive fauna documentation for [REGION-NAME]:

WILDLIFE OVERVIEW
- What major animal groups are represented?
- How many species in each group (mammals, birds, reptiles, amphibians, fish, invertebrates)?
- How does diversity compare to similar regions?
- What is the ratio of native to non-native species?

ENDEMIC SPECIES
- What animal species are found ONLY in this region?
- How did they evolve/become endemic?
- What are their conservation statuses?
- What makes them unique?
- Where exactly can they be found?

KEYSTONE SPECIES
- What species play critical ecological roles?
- How do they shape the ecosystem?
- What would happen if they disappeared?
- What is their current status?

CHARISMATIC MEGAFAUNA
- What large, visible animals draw attention?
- What is their conservation status?
- What is their cultural significance?
- Where can they be observed?

THREATENED FAUNA
- What species are listed as threatened or endangered?
- What are the primary threats to each?
- What conservation efforts are underway?
- What recovery successes have occurred?
- What species have been lost from the region?

INVASIVE SPECIES
- What non-native animals are causing problems?
- How did they arrive?
- What damage do they cause?
- What control efforts exist?

MIGRATION AND MOVEMENT
- What migratory species pass through or reside seasonally?
- What are the key migration routes?
- What stopover habitats are critical?
- How have patterns changed over time?

ECOLOGICAL RELATIONSHIPS
- What are the key predator-prey relationships?
- What species are critical for seed dispersal or pollination?
- What symbiotic relationships exist?
- How do animals shape the physical environment?

HUMAN-WILDLIFE INTERACTIONS
- What conflicts exist between humans and wildlife?
- What species were important to indigenous peoples?
- What traditional knowledge exists about wildlife?
- What hunting or fishing traditions exist?

WILDLIFE RESEARCH
- What major wildlife surveys have been conducted?
- Who were the key researchers?
- What discoveries were made here?
- What ongoing research is happening?
```

---

## Research Prompt - Individual Species

```
Research and compile documentation for [SPECIES-NAME] in [REGION-NAME]:

TAXONOMY AND IDENTIFICATION
- Scientific name and authority
- Common names (local, regional, indigenous)
- Class, order, family
- Subspecies if applicable
- How to identify (key features)
- Similar species and how to distinguish

PHYSICAL DESCRIPTION
- Body length, weight, wingspan (as applicable)
- Sexual dimorphism
- Coloration and markings
- Distinctive features
- Vocalizations

ECOLOGY
- Preferred habitat
- Elevation range
- Home range size
- Diet and foraging behavior
- Ecological role
- Predators and prey

DISTRIBUTION
- Range within the region (describe or reference map)
- Population status and estimates
- Historical vs. current range
- Seasonal distribution

BEHAVIOR
- Activity patterns (diurnal, nocturnal, etc.)
- Social structure
- Territorial behavior
- Communication methods
- Unusual behaviors

LIFE HISTORY
- Reproductive season
- Mating system
- Gestation/incubation
- Litter/clutch size
- Parental care
- Development and maturation
- Lifespan

CONSERVATION
- IUCN or regional conservation status
- Population trends
- Historical population changes
- Threats
- Protection efforts
- Success stories

HUMAN CONNECTIONS
- Traditional importance
- Cultural significance
- Discovery/research history
- Tourism value
- Conflicts with humans

INTERESTING FACTS
- What surprises people about this species?
- What unique behaviors does it exhibit?
- What stories are associated with it?
```

---

## Narrative Weighting Focus

For fauna documentation, prioritize:

| Criterion | Look For |
|-----------|----------|
| `[UNEXPECTED]` | Surprising behaviors, abilities, or discoveries |
| `[UNUSUAL]` | Endemic species, rare animals, unusual adaptations |
| `[TURNING]` | Conservation victories and defeats, population crashes and recoveries |
| `[HUMAN]` | Discovery stories, researchers, indigenous relationships, conservation heroes |
| `[PARADOX]` | Conflicting behaviors, animals that defy categories |

---

## Key Questions to Answer

### Uniqueness Questions
- What animals exist only here? `[UNUSUAL]`
- What adaptations evolved specifically for this region?
- What animal surprises researchers? `[UNEXPECTED]`

### Conservation Questions
- What species was brought back from the brink? `[TURNING]`
- What species was lost and what was learned?
- What conservation battle is being fought now?

### Behavior Questions
- What is the most unusual behavior documented here? `[UNUSUAL]`
- What animal has the most surprising ability? `[UNEXPECTED]`
- What ecological relationship is most critical?

### Human Connection Questions
- What animal was most important to indigenous peoples? `[HUMAN]`
- What discovery story is most compelling? `[HUMAN]`
- What researcher dedicated their life to a species here?

---

## Example Narrative-Weighted Findings

**High Narrative Weight:**
- "The population crashed to just 22 individuals in 1982—today there are over 5,000, making this one of conservation's greatest success stories." `[TURNING]` `[HUMAN]`
- "This bird mimics not just other birds but chainsaws, camera shutters, and car alarms with perfect accuracy." `[UNUSUAL]`
- "It was assumed extinct for 90 years until a game camera captured images of one in 2019." `[TURNING]` `[UNEXPECTED]`
- "Indigenous peoples had a taboo against hunting this animal, believing it carried the spirits of ancestors—this unintentional conservation may be why it survived." `[HUMAN]` `[PARADOX]`

**Supporting Context:**
- "The region supports 345 bird species, 89 mammal species, and 67 reptile species."
- "Migration peaks occur in April and October."

---

## Output Structure

### Primary Findings (High Narrative Weight)
Compelling wildlife stories and discoveries:
- [Finding] `[FLAG]` - Source

### Supporting Context (Essential Background)
Standard wildlife data:
- [Fact with source]

---

## Narrative Weighting Instructions

Apply these criteria to prioritize content with high narrative value:

1. **The Unexpected** `[UNEXPECTED]` — Surprising abilities or discoveries
2. **Paradox Resolution** `[PARADOX]` — Conflicting behaviors or survival strategies
3. **The Unusual** `[UNUSUAL]` — Endemic species, rare animals, behavioral oddities
4. **Human Interest** `[HUMAN]` — Researchers, indigenous connections, conservation heroes
5. **Turning Points** `[TURNING]` — Population crashes and recoveries, conservation milestones

### Output Format

**Primary Findings** (high narrative weight):
- [Fact with source] `[CRITERION-FLAG]`

**Supporting Context** (essential background):
- [Background fact with source]

Maintain factual accuracy. Narrative interest guides selection, never overrides truthfulness.

---

*Query template for fauna documentation*



