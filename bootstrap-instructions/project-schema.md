# Geographic Region Project Schema

## Overview

This document defines the organizational structure for cursor.ai projects focused on documenting geographic regions. Each project represents a single region and serves as both a comprehensive content database and source material for generating derivative content such as documentary episodes, educational materials, and other commentary.

## Design Principles

- **Single Region Focus**: Each project contains information about one geographic region
- **Narrative-Weighted Research**: Content prioritizes engaging, memorable details over dry facts
- **Content Promotion Path**: Content flows from research → drafts → docs as it is vetted
- **Clear Separation**: Core vetted content (docs/) is separated from work-in-progress (drafts/) and reference materials (library/)
- **Reusability**: Core content database serves as foundation for multiple derivative works (commentaries/)
- **Comprehensive Coverage**: Schema covers geology, geography, natural history, human history, and significant figures

-----

## Top-Level Directory Structure

```
/project-root/
├── docs/                    # Vetted core content database
├── drafts/                  # Unvetted preliminary versions
├── library/                 # Reference materials & sources
├── research/                # Inbox for new uncategorized content
├── commentaries/            # Generated/derivative content
├── templates/               # Document templates
├── queries/                 # Research query templates
└── bootstrap-instructions/  # Project setup documentation
```

-----

## `/docs/` - Core Content Database

The `/docs/` directory contains all vetted, finalized content about the region. This is the authoritative source of information for the project.

### Subdirectories:

#### `/docs/overview/`

Regional overview and summary documents.

**Purpose**: High-level summaries and comprehensive regional documentation

**File naming**: `[region-name].md`, `[region-name]-extended-overview-part-[X].md`

**Content includes**:
- Basic geographic information
- Key facts and statistics
- Summary of major sections
- Narrative highlights
- Cross-references to detailed documents

-----

#### `/docs/geology/`

Geological documentation including formations, tectonic history, mineral resources, and feature-specific documents.

**Purpose**: Document the deep geological foundations and processes of the region through a multi-document structure.

**Multi-Document Structure** (Recommended):

| Document Type | Length | Purpose |
|---------------|--------|---------|
| `[region]-geology.md` | ~500-550 lines | Main comprehensive overview |
| `[feature-name].md` | ~200-450 lines | Individual geological features (variable by narrative value) |

**File naming**: `[region-name]-geology.md`, `[feature-name].md`

**Main Overview Content includes**:
- Narrative Highlights table with flags
- Tectonic setting and plate history
- Geological timeline (era by era)
- Rock types and named formations
- Mineral resources
- Soil composition
- Geological hazards (with specific events)
- Notable features summary table (linking to individual docs)
- Research history and key geologists

**Feature Document Structure**:

Each notable geological feature gets its own document. Length varies by narrative richness:

| Narrative Value | Line Target | Criteria |
|-----------------|-------------|----------|
| **Very High** | ~350-450 lines | Multiple paradoxes; superlatives; rich human connection |
| **High** | ~250-350 lines | Strong narrative hooks; visible processes |
| **Medium** | ~200-250 lines | Standard features with clear story |

**Feature Document Content includes**:
- Quick Facts table
- Narrative Highlights table
- **Deep Time Context** section (when formed, how exposed, ongoing processes)
- Formation explanation with accessible science
- **Geology-Human Connection** section (discovery, climbing, indigenous knowledge)
- Viewing/access information
- Cross-references to related features

**Deep Time Context** (Required for each feature):
Document the feature's history through time:
- When the rock crystallized/deposited
- How it was exposed (erosion, uplift, glaciation)
- How it was shaped (weathering, glacial carving, exfoliation)
- Ongoing processes (rockfall, weathering, erosion rates)

**Geology-Human Connections** (Required where applicable):
- Discovery and naming history (who, when)
- How indigenous peoples understood the feature
- How climbers/visitors use geological knowledge
- How geology enables or constrains human activity

**Type Locality Documentation**:
If the region contains **type localities** (where rock types were first described), document this prominently—it's inherently `[UNUSUAL]`.

**Process Explanations**:
For key geological processes visible in the region, explain the counter-intuitive aspects:
- Exfoliation: Domes form from expansion, not compression `[PARADOX]`
- Glacial carving: Different glacier sizes create different features
- Hanging valleys: Why tributary waterfalls exist

**Narrative Focus**: 
- Catastrophic events `[TURNING]`
- Unusual formations and superlatives `[UNUSUAL]`
- Discovery stories and scientists `[HUMAN]`
- Counter-intuitive processes `[PARADOX]`
- Geology enabling human activity `[UNEXPECTED]`

-----

#### `/docs/geography/`

Geographic documentation including topography, climate, and hydrology.

**Purpose**: Document the physical geography and environmental conditions

**File naming**: `[region-name]-geography.md`, `[feature-name].md`

**Content includes**:
- Topography and elevation profiles
- Climate zones and weather patterns
- Hydrological systems (rivers, lakes, aquifers)
- Ecosystem types and biomes
- Borders and boundaries
- Microclimates and unusual conditions

**Narrative Focus**: Extreme weather `[UNUSUAL]`, climate paradoxes `[PARADOX]`, boundary disputes `[TURNING]`

-----

#### `/docs/evolutionary-history/`

Deep time documentation from Precambrian through Cenozoic.

**Purpose**: Document the evolutionary and paleontological history

**Three-Document Structure** (Recommended):

| Document | Length | Purpose |
|----------|--------|---------|
| `[region-name]-deep-time.md` | ~400-450 lines | Main comprehensive overview |
| `cenozoic-era.md` | ~300-350 lines | Detailed Age of Mammals and recent history |
| `fossil-record.md` | ~250-300 lines | Paleontological focus and proxy records |

**File naming**: `[region-name]-deep-time.md`, `cenozoic-era.md`, `fossil-record.md`

**Content includes**:
- Era-by-era geological and biological history
- Mass extinction impacts
- Fossil record and paleoenvironments (or explanation of absence)
- Endemic evolutionary lineages and living fossils
- Paleoclimate reconstructions
- **Proxy records** for fossil-poor regions (dendrochronology, lake cores, pollen)

**Rock Type Considerations**:

| Rock Type | Fossil Potential | Documentation Approach |
|-----------|------------------|------------------------|
| **Sedimentary** | High | Focus on fossil sites and discoveries |
| **Igneous (granite, basalt)** | None | Frame the "problem"; use proxy records |
| **Metamorphic** | Low (usually destroyed) | Document roof pendants, regional context |
| **Mixed** | Variable | Identify fossil-bearing units |

**The "Problem" Framing**:
For regions with limited fossil records, frame the absence as the story itself:
- "The Granite Problem" (igneous regions)
- "The Metamorphic Gap" (highly altered rocks)
- "The Erosion Story" (heavily weathered terrain)
- "The Glacial Erasure" (ice-scoured landscapes)

**Proxy Records** (for fossil-poor regions):

| Proxy | Information Provided | Typical Range |
|-------|---------------------|---------------|
| Tree rings (dendrochronology) | Climate, fire, precipitation | Up to ~10,000 years |
| Lake sediment cores | Vegetation, fire, climate | Up to ~50,000 years |
| Pollen records | Plant communities | Up to ~50,000 years |
| Glacial features | Ice extent, timing | Up to millions of years |
| Living fossils | Evolutionary history | Millions of years |

**Living Fossils Section** (required):
Document species representing ancient lineages that persist in the region:
- Genus/family age and evolutionary history
- Why they survived while relatives went extinct
- Connection to modern ecosystems
- Conservation significance

**Narrative Focus**: 
- Extinction survivors `[UNUSUAL]`
- Discovery stories `[HUMAN]`
- Catastrophic events `[TURNING]`
- Why fossils are absent `[PARADOX]`
- Fossil finds that changed understanding `[UNEXPECTED]`

-----

#### `/docs/natural-history/`

Flora and fauna documentation organized in subdirectories. Natural history is one of the most substantial phases, producing 16-22 documents (~4,900-7,400 lines).

##### `/docs/natural-history/flora/`

Plant species documentation.

**Purpose**: Document the botanical diversity of the region

**Multi-Document Structure** (Recommended):

| Document Type | Count | Lines | Purpose |
|---------------|-------|-------|---------|
| `[region]-flora-overview.md` | 1 | ~400 | Vegetation zones, endemic summary, species index |
| `[species-name].md` (high-profile) | 2-3 | ~350-400 each | Endemic, conservation, flagship species |
| `[species-name].md` (standard) | 3-5 | ~250-300 each | Ecologically important species |
| **Flora Total** | **6-9** | **~1,850-3,100** | |

**File naming**: `[region-name]-flora-overview.md`, `[species-name].md`

**Overview Content includes**:
- Basic Information table (species count, vegetation types, endemics)
- Narrative Highlights table
- Major plant communities/vegetation zones
- Endemic and notable species table (linking to profiles)
- Conservation status summary
- Indigenous ethnobotany overview
- Research history

**Species Profile Content includes**:
- **Biographical Lead Quote** (from project figure, with citation)
- Basic Information table
- Narrative Highlights table
- Physical description and identification
- Ecology and habitat
- Conservation status
- Cultural significance
- Where/when to observe

**Species Selection Criteria**:

| Priority | Criterion | Flag |
|----------|-----------|------|
| 1 | Endemic/regional specialty | `[UNUSUAL]` |
| 2 | Conservation story | `[TURNING]` |
| 3 | Indigenous connection | `[HUMAN]` |
| 4 | Ecological keystone | — |
| 5 | Climate indicator | `[TURNING]` |
| 6 | Visitor recognition | — |

**Narrative Focus**: Endemic origins `[UNUSUAL]`, conservation turning points `[TURNING]`, ethnobotanical uses `[HUMAN]`

##### `/docs/natural-history/fauna/`

Animal species documentation.

**Purpose**: Document the zoological diversity of the region

**Multi-Document Structure** (Recommended):

| Document Type | Count | Lines | Purpose |
|---------------|-------|-------|---------|
| `[region]-fauna-overview.md` | 1 | ~400 | Wildlife groups, conservation summary, species index |
| `[species-name].md` (high-profile) | 3-4 | ~350-400 each | Endemic, recovery stories, flagship |
| `[species-name].md` (standard) | 5-8 | ~250-300 each | Ecologically important species |
| **Fauna Total** | **9-13** | **~2,700-4,400** | |

**File naming**: `[region-name]-fauna-overview.md`, `[species-name].md`

**Overview Content includes**:
- Basic Information table (species counts by class, endemics)
- Narrative Highlights table
- Mammals summary
- Birds summary
- Reptiles/amphibians summary
- Fish/aquatic summary (if applicable)
- Endemic and notable species table (linking to profiles)
- Conservation status summary
- Human-wildlife interactions overview
- Indigenous connections
- Research history

**Species Profile Content includes**:
- **Biographical Lead Quote** (from project figure, with citation)
- Basic Information table
- Narrative Highlights table
- Physical description and identification
- Behavior and ecology
- Conservation status and history
- Human interactions
- Cultural significance
- Where/when to observe
- Safety considerations (if applicable)

**Taxonomic Balance Guide**:

| Group | Target | Notes |
|-------|--------|-------|
| Mammals | 3-5 | Include predator, large herbivore, small mammal |
| Birds | 2-4 | Include raptor, songbird, or specialty |
| Fish | 1-2 | Native aquatic species (if applicable) |
| Other | 0-2 | Regionally iconic reptiles, amphibians, invertebrates |

**Species Selection Criteria**:

| Priority | Criterion | Flag |
|----------|-----------|------|
| 1 | Endemic subspecies | `[UNUSUAL]` |
| 2 | Conservation milestone | `[TURNING]` |
| 3 | Keystone predator/herbivore | — |
| 4 | Indigenous significance | `[HUMAN]` |
| 5 | Human-wildlife interface | `[HUMAN]` |
| 6 | Climate sentinel | `[TURNING]` |
| 7 | Charismatic megafauna | — |

**Narrative Focus**: Unusual behaviors `[UNUSUAL]`, recovery stories `[TURNING]`, research discoveries `[HUMAN]`

##### Biographical Lead Quotes (Required for all species profiles)

Each species profile opens with an inspiring quote from a project biographical figure:

```markdown
> "[Quote about the species or its ecosystem]"
> — **[Figure Name]**, *[Source Title]* ([Year])
```

**Quote Priority**:
1. Direct species mention (highest priority)
2. Related species or group
3. Habitat/ecosystem reference
4. General nature/wilderness reflection

**Important**: Complete `/docs/biographies/` before natural history documentation to enable lead quote research.

-----

#### `/docs/human-history/`

Historical documentation from prehistory to present.

**Purpose**: Document the human story of the region

**File naming**: `[region-name]-history.md`, `[era-name].md`

**Content includes**:
- Archaeological prehistory
- Indigenous peoples and cultures
- Colonial/contact period
- Modern development
- Significant events

**Narrative Focus**: Turning points `[TURNING]`, overlooked figures `[HUMAN]`, revisionist discoveries `[UNEXPECTED]`

-----

#### `/docs/cultural-organization/`

Current governance, demographics, and social organization.

**Purpose**: Document the contemporary human organization of the region

**File naming**: `[region-name]-cultural-overview.md`, `municipalities/[name].md`

**Content includes**:
- Governance structure
- Administrative divisions
- Population demographics
- Economic sectors
- Infrastructure
- Cultural institutions

**Narrative Focus**: Demographic paradoxes `[PARADOX]`, political turning points `[TURNING]`, unusual governance `[UNUSUAL]`

-----

#### `/docs/biographies/`

Biographies of 4-8 historically significant figures.

**Purpose**: Document individuals who shaped or represent the region

**File naming**: `[figure-name].md`, `[figure-name]-short.md`

**Content includes**:
- Basic biographical information
- Connection to the region
- Major contributions
- Character-revealing details
- Legacy and commemoration

**Selection Categories**:
- Indigenous leaders
- Explorers and scientists
- Political figures
- Cultural icons
- Conservationists

**Narrative Focus**: Character-revealing moments `[HUMAN]`, unexpected connections `[UNEXPECTED]`, life turning points `[TURNING]`

-----

#### `/docs/landmarks/`

Natural and cultural landmarks.

**Purpose**: Document significant locations within the region

**File naming**: `[landmark-name].md`

**Content includes**:
- Location and access
- Physical description
- Significance (geological, historical, cultural)
- Discovery or designation history
- Current status
- Visitor information

**Narrative Focus**: Formation stories `[UNUSUAL]`, historical events `[TURNING]`, discovery tales `[HUMAN]`

-----

#### `/docs/timeline/`

Chronological organization of the region's history.

**Purpose**: Provide temporal context and easy navigation by date

**File naming**: `[region-name]-timeline.md`, `[era-name]-timeline.md`

**Content includes**:
- Geological timeline
- Evolutionary timeline
- Human history timeline
- Significant events by date
- Cross-references to detailed docs

-----

#### `/docs/influences/`

Cultural influences and connections.

**Purpose**: Document how the region influenced and was influenced by broader contexts

**File naming**: `[influence-name].md`

**Content includes**:
- Migration patterns
- Trade and cultural exchange
- Colonial influences
- Modern globalization effects
- Regional identity formation

-----

#### `/docs/media/`

References to visual and multimedia content.

**Subdirectories**:
- `/media/maps/` - Cartographic resources
- `/media/photos/` - Image references and descriptions
- `/media/documentaries/` - Films about the region
- `/media/videos/` - Other video content

**Content includes**:
- Title and description
- Source and credits
- Date and context
- Links or file references
- Usage notes

-----

## `/drafts/` - Work in Progress

The `/drafts/` directory mirrors the complete structure of `/docs/` and contains preliminary, unvetted versions of content.

### Structure:

```
/drafts/
├── overview/
├── geology/
├── geography/
├── evolutionary-history/
├── natural-history/
│   ├── flora/
│   └── fauna/
├── cultural-organization/
│   └── municipalities/
├── human-history/
├── biographies/
├── landmarks/
├── timeline/
├── influences/
└── media/
```

### Purpose:
- Hold works-in-progress before finalization
- Allow for review and editing
- Provide clear promotion path: drafts → docs

### Workflow:
1. New content created in `/drafts/[subdirectory]/`
2. Content reviewed, fact-checked, edited
3. Narrative weighting verified
4. Sources attributed
5. Vetted content moved to `/docs/[subdirectory]/`

### Frontmatter:
Use `status: draft` in YAML frontmatter to indicate draft status

-----

## `/library/` - Reference Materials

The `/library/` directory contains source materials and documentation.

### Subdirectories:

| Directory | Purpose |
|-----------|---------|
| `academic/` | Scholarly papers, studies, dissertations |
| `articles/` | Journalism, magazine features, news reports |
| `books/` | Book excerpts, regional histories, guides |
| `essays/` | Opinion pieces, commentary |
| `geological-surveys/` | Official geological survey documents |
| `maps/` | Historical and modern cartography |
| `archaeological-records/` | Excavation reports, artifact catalogs |
| `municipal-records/` | Government documents, census data |
| `natural-surveys/` | Flora/fauna inventories, ecological studies |
| `historical-documents/` | Historical letters, documents, records |
| `primary-sources/` | Original documents and first-hand accounts |
| `government-announcements/` | Official statements and press releases |
| `interviews/` | Interview transcripts and recordings |

### Purpose:
- Maintain source materials for fact-checking
- Preserve primary sources
- Provide attribution for information in `/docs/`
- Support research and content creation

-----

## `/research/` - Inbox

The `/research/` directory is a flat, unorganized inbox for new content.

### Purpose:
- Temporary holding area for new materials
- No schema requirements
- Quick capture of information

### Workflow:
1. New materials added with descriptive filenames
2. Content reviewed and sorted
3. Materials moved to `/drafts/` or `/library/`
4. Or deleted if not needed

-----

## `/commentaries/` - Derivative Content

The `/commentaries/` directory contains generated content using the core database.

### Structure:

```
/commentaries/
├── templates/
│   ├── episode-template.md
│   ├── script-template.md
│   └── render-instructions-template.md
└── [show-name]/
    ├── show-config.md
    ├── research/
    └── seasons/
        └── season-##/
            └── episode-###/
                ├── script.md
                ├── render-instructions.md
                ├── source-references.md
                └── output/
```

### Components:

- **Episode templates**: Structure for commentary episodes
- **Script templates**: Format for narration scripts
- **Render instructions**: Production guidelines including pronunciation guides
- **Show config**: Series-level settings and style guides

-----

## Metadata and Frontmatter

Standard YAML frontmatter for markdown files:

```yaml
---
title: [Document Title]
type: [overview|geology|geography|species|biography|landmark|etc.]
region: [REGION-NAME]
date: [YYYY-MM-DD]
tags: [tag1, tag2, tag3]
status: [vetted|draft|research]
sources: [links to library files]
related: [links to other docs]
narrative_flags: [UNEXPECTED, UNUSUAL, TURNING, HUMAN, PARADOX]
contributors: []
last_updated: [YYYY-MM-DD]
---
```

-----

## Narrative Research Methodology

All content should apply narrative weighting criteria:

| Flag | Criterion | Description |
|------|-----------|-------------|
| `[UNEXPECTED]` | The Unexpected | Facts contradicting common assumptions |
| `[PARADOX]` | Paradox Resolution | Details reconciling conflicting accounts |
| `[UNUSUAL]` | The Unusual | Outliers, anomalies, statistical rarities |
| `[HUMAN]` | Human Interest | Personal stories, character-revealing details |
| `[TURNING]` | Turning Points | Moments where outcomes hung in balance |

See `queries/narrative-research-methodology.md` for complete methodology.

-----

## File Naming Conventions

### General Principles:
- Use lowercase letters
- Use hyphens (kebab-case) not underscores or spaces
- Be descriptive but concise
- Include dates when relevant (YYYY-MM-DD format)

### Examples:

**Overview**: `yellowstone.md`, `yellowstone-extended-overview-part-1.md`

**Geology**: `yellowstone-geology.md`, `old-faithful-geyser.md`

**Species**: `american-bison.md`, `lodgepole-pine.md`

**Biography**: `john-colter.md`, `john-colter-short.md`

**Landmarks**: `grand-prismatic-spring.md`

**Timeline**: `yellowstone-timeline.md`

-----

## Cross-Referencing Best Practices

### Internal Links:
- Use relative paths: `[Grand Prismatic](../landmarks/grand-prismatic-spring.md)`
- Link between related documents
- Create web of connections

### Source Attribution:
- Always link to `/library/` sources
- Use `sources:` field in frontmatter
- Maintain clear provenance for all facts

### Narrative Flag Links:
- Link narrative-flagged content to supporting context
- Create "See Also" sections for related compelling content

-----

## Workflow Examples

### Adding New Species Documentation

1. **Research**: Add field guides, papers to `/library/natural-surveys/`
2. **Draft**: Create `/drafts/natural-history/fauna/[species].md`
3. **Apply Narrative Weighting**: Flag compelling content
4. **Review**: Fact-check against sources
5. **Promote**: Move to `/docs/natural-history/fauna/[species].md`

### Creating a Biography

1. **Research**: Gather sources in `/library/`
2. **Draft**: Create `/drafts/biographies/[figure-name].md`
3. **Narrative Focus**: Identify `[HUMAN]` and `[TURNING]` content
4. **Cross-Reference**: Link to human history documents
5. **Review**: Verify facts and sources
6. **Promote**: Move to `/docs/biographies/`

-----

## Customization Notes

This schema can be adapted based on:

- **Region type**: National parks may emphasize natural history; urban regions may emphasize cultural organization
- **Scale**: Larger regions may need more granular organization
- **Research availability**: Some sections may be limited by available sources
- **Output goals**: Documentary vs. educational content may emphasize different sections

-----

## Quick Reference

### Content Flow:
```
New Material → /research/ → /drafts/ → /docs/ → /commentaries/
                    ↓
               /library/ (reference materials)
```

### Key Principles:
1. One project per region
2. Mirror structure between `/docs/` and `/drafts/`
3. Apply narrative weighting throughout
4. Always cite sources from `/library/`
5. Use consistent frontmatter metadata
6. Link related documents for navigation

-----

## Version History

- **v1.0** (2025-11-29): Initial schema definition for geographic regions

-----

*This schema is a living document and should be updated as the project evolves.*
