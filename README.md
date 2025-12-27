# Taos, New Mexico Regional Concordance

## Overview

This project documents the comprehensive natural and human history of Taos, New Mexico, organized according to the schema defined in `bootstrap-instructions/project-schema.md`. The documentation follows a **narrative-weighted research methodology** to produce engaging, memorable content—not a dry recounting of facts.

## Region Type

High desert valley / Cultural-historical region

## Geographic Coordinates

- **Latitude**: 36.4°N
- **Longitude**: 105.6°W
- **Area**: ~2,203 sq miles (Taos County)
- **Boundaries**: Bounded by Sangre de Cristo Mountains (east), Rio Grande Gorge (west), extending from Questa (north) to Picuris Pueblo area (south)

## Project Structure

- **`/docs/`** - Vetted, authoritative content about Taos, New Mexico
- **`/drafts/`** - Work-in-progress content being developed
- **`/library/`** - Reference materials and source documents
- **`/research/`** - Inbox for new, uncategorized materials
- **`/commentaries/`** - Derivative works (documentaries, podcasts, etc.)
- **`/templates/`** - Template files for creating new documents
- **`/queries/`** - Research query templates for content development
- **`/bootstrap-instructions/`** - Project setup and schema documentation

---

## Template Instantiation

### How to Create a New Region Project

To instantiate this template for a specific region, copy the entire `region-template/` directory to a new location and use the following query:

**Template Instantiation Query:**
```
Instantiate this region-template project for [REGION-NAME]. 
Replace all [PLACEHOLDER] values throughout the project with specific 
details for this region. The primary deep-dive topic should be 
[PRIMARY-TOPIC] (e.g., geology, human history, biodiversity). 
Update README.md, BOOTSTRAP-QUERIES.md, and create the initial 
region overview draft in /drafts/overview/.
```

**Example usage:**
> "Instantiate this region-template project for Yellowstone National Park. Replace all placeholder values with specific details for this region. The primary deep-dive topic should be geology and geothermal features."

---

## Narrative Research Methodology

This project emphasizes **narrative-weighted research** to produce content that is both accurate and engaging. All research applies five key criteria:

| Criterion | Description | Flag |
|-----------|-------------|------|
| **The Unexpected** | Facts contradicting common assumptions | `[UNEXPECTED]` |
| **Paradox Resolution** | Details reconciling conflicting accounts | `[PARADOX]` |
| **The Unusual** | Outliers, anomalies, statistical rarities | `[UNUSUAL]` |
| **Human Interest** | Personal stories, emotional stakes, character details | `[HUMAN]` |
| **Turning Points** | Moments where outcomes hung in balance | `[TURNING]` |

See `queries/narrative-research-methodology.md` for complete methodology.

---

## Deep Dive Topic: Human History, Indigenous Culture, and Art/Literary Heritage

This project gives special focus to Taos, New Mexico's **Human History, Indigenous Culture, and Art/Literary Heritage**, providing detailed analysis equivalent in depth and complexity to comprehensive academic documentation.

### Human History, Indigenous Culture, and Art/Literary Heritage Coverage Includes:
- Comprehensive overview and context
- Detailed technical/scientific documentation
- Historical development and changes over time
- Key figures and their contributions
- Current status and conservation/preservation efforts
- Narrative highlights and engaging stories

---

## Documentation Best Practices

### Two-Tier Overview System

This project uses a **two-tier overview system** for comprehensive regional coverage:

| Type | Template | Lines | Files | Use Case |
|------|----------|-------|-------|----------|
| **Short Overview** | `region-short-overview-template.md` | ~100-150 | 1 | Quick reference |
| **Extended Overview** | `region-extended-overview-template.md` | ~1000+ | 10 | Comprehensive |

### Why 10 Parts for Extended Overviews?

Extended regional documentation exceeding 1,000 lines is:
- **Prone to interruption** during AI-assisted creation
- **Difficult to review** as a single massive file
- **Hard to track progress** when incomplete

The **10-part structure** provides:
- ✅ Checkpoint timestamps for recovery
- ✅ Manageable file sizes (~100 lines each)
- ✅ Clear handoff points between agents
- ✅ Easier review and editing

### Part Structure

| Part | Content |
|------|---------|
| 1 | Basic Info, Geographic Overview, Boundaries |
| 2 | Geological Foundation and Tectonic History |
| 3 | Geography: Topography, Climate, Hydrology |
| 4 | Evolutionary History and Paleontology |
| 5 | Natural History: Flora Overview |
| 6 | Natural History: Fauna Overview |
| 7 | Human History: Prehistory to Colonial Era |
| 8 | Human History: Modern Era to Present |
| 9 | Cultural Organization and Demographics |
| 10 | Significant Figures, Legacy, Sources |

### Timestamp Checkpoints

Each extended overview part **must end** with:

```markdown
*Part X completed at YYYY-MM-DDTHH:MM:SSZ*

*Continue to [Part Y: Section Title](region-name-extended-overview-part-Y.md)*
```

---

## Getting Started

### Phase 1: Foundation
1. Add source materials to `/research/` (surveys, studies, historical documents)
2. Create **short overview** in `/drafts/overview/[region-name].md`
3. Create **extended overview** in 10 parts using `region-extended-overview-template.md`
4. Use `queries/region-overview-query.md` as research framework

### Phase 2: Geology Deep Dive

Geology documentation uses a **multi-document structure**: one main overview plus feature-specific documents.

| Document Type | Target Length | Content Focus |
|---------------|---------------|---------------|
| `[region]-geology.md` | ~500-550 lines | Main comprehensive overview |
| `[feature-name].md` | ~200-450 lines | Individual geological features (length varies by narrative richness) |

**Steps:**
1. Create main geology overview: `/drafts/geology/[region]-geology.md`
2. Use `queries/geological-survey-query.md` as research framework
3. Identify 4-8 notable geological features for individual documentation
4. Create feature documents with length proportional to narrative value:
   - **High narrative value** (multiple `[PARADOX]`, `[UNUSUAL]`, `[HUMAN]`): ~350-450 lines
   - **Medium narrative value**: ~250-300 lines
   - **Standard features**: ~200-250 lines
5. Include **Deep Time Context** for each feature (when rock formed, how exposed, ongoing processes)
6. Document **Geology-Human Connections** (climbing, discovery, indigenous knowledge)
7. Cross-reference features in main overview table

**Narrative Weighting for Geology:**

| Flag | Look For in Geological Features |
|------|----------------------------------|
| `[PARADOX]` | Counter-intuitive formation processes; "missing" features that were never there |
| `[UNUSUAL]` | Superlatives (largest, oldest, only); unique rock types; type localities |
| `[UNEXPECTED]` | Geology that enabled human activities; features that surprised scientists |
| `[TURNING]` | Views/evidence that proved theories; catastrophic events; ongoing processes |
| `[HUMAN]` | Discovery stories; how climbers/visitors use geological knowledge; indigenous names |

**Feature Document Selection Criteria:**
- Does the feature have a compelling story or paradox?
- Is it a type locality or superlative?
- Does geology connect to human activity (climbing, tourism, discovery)?
- Can visitors see and experience the geology directly?

### Phase 3: Geography Documentation
1. Document topography, climate, and hydrology
2. Use `queries/geographical-analysis-query.md` for research
3. Create ecosystem documentation
4. Map hydrological systems

### Phase 4: Evolutionary History

Evolutionary history documentation uses a **three-document structure** for comprehensive coverage:

| Document | Target Length | Content Focus |
|----------|---------------|---------------|
| `[region]-deep-time.md` | ~400-450 lines | Main comprehensive overview: all eras, endemic lineages, climate history |
| `cenozoic-era.md` | ~300-350 lines | Detailed Cenozoic: mammals, glaciation, ecosystem development |
| `fossil-record.md` | ~250-300 lines | Paleontological focus: sites, discoveries, proxy records |

**Steps:**
1. Use `queries/evolutionary-history-query.md` for research framework
2. Create main deep-time document with Narrative Highlights table
3. Create Cenozoic detail document (most relevant to modern ecosystems)
4. Create fossil record document—frame around the region's "problem" (e.g., "The Granite Problem" for igneous regions, "The Marine Record" for coastal regions)
5. For fossil-poor regions, document **proxy records**: dendrochronology, lake sediments, pollen cores
6. Include **Living Fossils** section for ancient lineages that persist today
7. Update Part 4 of extended overview with cross-references to detailed documents

**Narrative Weighting for Evolution:**

| Flag | Look For in Evolutionary History |
|------|----------------------------------|
| `[UNEXPECTED]` | Fossil discoveries that changed understanding; life where none expected |
| `[PARADOX]` | Why fossils are absent (granite, erosion); conflicting evidence resolved |
| `[UNUSUAL]` | Endemic species; living fossils; unique adaptations; paleoendemic refugia |
| `[TURNING]` | Mass extinctions; glacial cycles; climate catastrophes; human arrival |
| `[HUMAN]` | Discovery stories; paleontologists; dendrochronology researchers |

### Phase 5: Natural History

Natural history is one of the most substantial documentation phases, producing 16-22 documents totaling ~4,900-7,400 lines.

#### 5.1 Preparation
1. Research biographical quotes from figures in `/docs/biographies/` for lead quotes
2. Plan species selection covering habitat diversity and taxonomic balance

#### 5.2 Flora Documentation (~7-9 documents)
| Document Type | Count | Lines | Notes |
|---------------|-------|-------|-------|
| Flora Overview | 1 | ~400 | Vegetation zones, endemic summary |
| High-Profile Species | 2-3 | ~350-400 each | Endemic, conservation stories |
| Standard Species | 3-5 | ~250-300 each | Ecologically important |

**Species Selection Criteria**: Endemic/regional specialty, conservation story `[TURNING]`, indigenous connection `[HUMAN]`, ecological keystone, climate indicator, visitor recognition.

#### 5.3 Fauna Documentation (~9-13 documents)
| Document Type | Count | Lines | Notes |
|---------------|-------|-------|-------|
| Fauna Overview | 1 | ~400 | Wildlife groups, conservation summary |
| High-Profile Species | 3-4 | ~350-400 each | Endemic, recovery stories |
| Standard Species | 5-8 | ~250-300 each | Ecologically important |

**Taxonomic Balance**: Mammals (3-5), Birds (2-4), Fish (1-2 if applicable), Other (0-2).

**Species Selection Criteria**: Endemic subspecies, conservation milestone `[TURNING]`, keystone predator/herbivore, indigenous significance `[HUMAN]`, human-wildlife interface, climate sentinel, charismatic megafauna.

#### 5.4 Biographical Lead Quotes (Required)

Each species profile opens with an inspiring quote from a project biographical figure:

```markdown
> "[Quote about the species or its ecosystem]"
> — **[Figure Name]**, *[Source Title]* ([Year])
```

**Quote Priority**:
1. Direct species mention
2. Related species or group
3. Habitat/ecosystem reference
4. General nature/wilderness reflection

#### 5.5 Execution Order
1. Research quotes from biographies
2. Create flora overview → fauna overview
3. Create high-profile species (flora, then fauna)
4. Create standard species (flora, then fauna)
5. Update overviews with cross-references

### Phase 6: Human History
1. Document archaeological prehistory
2. Document historical periods using era templates
3. Use `queries/human-history-query.md`
4. Track significant events and developments

### Phase 7: Cultural Organization
1. Document current governance structure
2. Create municipality profiles
3. Document demographics and economic sectors
4. Use `queries/cultural-analysis-query.md`

### Phase 8: Significant Figures (4-8 Biographies)
1. Identify 4-8 historically significant people
2. Create biographies using `templates/significant-figure-template.md`
3. Use `queries/significant-figure-biography-query.md`
4. **REQUIRED**: Include "[REGION-NAME] Record" section with:
   - Arrival dates and residency timespan
   - Chronology of visits/activities with dates
   - Works created or related to region (with dates)
   - Notable encounters with other significant figures
5. Cross-reference with human history section and other biographies

### Phase 9: Review and Promotion
1. Fact-check and verify all draft content
2. Move vetted content from `/drafts/` to `/docs/`
3. Maintain cross-references and links
4. Ensure source attribution for all claims

### Phase 10: Commentary Creation
1. Plan documentary or podcast episodes based on `/docs/` content
2. Use templates in `/commentaries/templates/`
3. Create episode structure and scripts
4. Generate derivative content using core database

---

## Content Development Queries

### Short Regional Overview
**Prompt**: "Create a short overview (~100-150 lines) for Taos, New Mexico using the region-short-overview-template.md format. Include basic information table, geographic summary, quick facts, and links to extended documentation. Apply narrative weighting to highlight engaging content."

### Extended Overview (10 Parts)
**Prompt**: "Create the extended overview for Taos, New Mexico in 10 parts following region-extended-overview-template.md. Start with Part 1 (Basic Info, Geographic Overview, Boundaries). End each part with a timestamp checkpoint. Apply narrative weighting criteria throughout."

### Geological Survey
**Prompt**: "Research and document the geology of Taos, New Mexico using the geological-survey-query.md template. Focus on tectonic history, rock formations, mineral resources, and geological hazards. Flag all content meeting narrative weighting criteria."

### Natural History Documentation
**Prompt**: "Document the flora and fauna of Taos, New Mexico using the flora-documentation-query.md and fauna-documentation-query.md templates. Prioritize endemic species, unusual behaviors, and conservation turning points."

### Significant Figure Biography
**Prompt**: "Create a biography for [FIGURE-NAME], historically significant to Taos, New Mexico. Use significant-figure-biography-query.md template. Include a 'Taos, New Mexico Record' section with: arrival dates, residency timeline, works created/related to region (with dates), significant activities, and notable encounters with other documented figures. Emphasize character-revealing moments and unexpected connections to the region."

---

## Reference Documents

- [Project Schema](bootstrap-instructions/project-schema.md) - Complete organizational structure
- [Setup Instructions](bootstrap-instructions/cursor-prompt-setup.md) - How this project was initialized
- [Narrative Methodology](queries/narrative-research-methodology.md) - Research weighting criteria
- Query Templates in `/queries/` - Research frameworks for content development
- Document Templates in `/templates/` - Standard formats for different content types

---

## Status

- **Created**: December 24, 2025
- **Last Updated**: December 24, 2025
- **Template Version**: 1.0 (November 2025)
- **Documents in `/docs/`**: 0
- **Documents in `/drafts/`**: 0
- **Primary Deep Dive**: Human/Indigenous History & Arts

## Next Steps

1. ✅ Project structure created
2. Create initial Taos, New Mexico overview in `/drafts/overview/taos.md`
3. Begin adding source materials to `/library/`
4. Create geology documentation in `/drafts/geology/`
5. Document geography and climate
6. Research evolutionary and paleontological history
7. **Create 4-8 significant figure biographies (needed for lead quotes)**
8. **Document flora: 1 overview + 6-8 species profiles (~7-9 documents)**
9. **Document fauna: 1 overview + 8-12 species profiles (~9-13 documents)**
10. Compile human history from prehistory to present
11. Document current cultural organization

---

## Key Directories

### `/docs/`
- `overview/` - Regional overview and summary documents
- `geology/` - Rock formations, tectonics, minerals, soils
- `geography/` - Topography, hydrology, climate, ecosystems
- `evolutionary-history/` - Deep time documentation by era
- `natural-history/flora/` - Plant species documentation
- `natural-history/fauna/` - Animal species documentation
- `cultural-organization/` - Governance, municipalities, demographics
- `human-history/` - Archaeological to modern historical narrative
- `biographies/` - 4-8 historically significant figures
- `landmarks/` - Natural and cultural landmarks
- `timeline/` - Geological and human timeline documents
- `influences/` - Cultural influences, migration patterns
- `media/` - Maps, photos, documentaries, videos

### `/library/`
Reference materials including:
- `academic/` - Scholarly papers and studies
- `articles/` - Journalism and feature articles
- `books/` - Regional histories and natural guides
- `geological-surveys/` - Official geological survey documents
- `maps/` - Historical and modern cartography
- `archaeological-records/` - Excavation reports, artifact catalogs
- `municipal-records/` - Government documents, census data
- `natural-surveys/` - Flora/fauna inventories, ecological studies

### `/templates/`
Document templates:
- `region-overview-template.md` - Basic regional summary
- `region-short-overview-template.md` - Quick reference overview
- `region-extended-overview-template.md` - Comprehensive (10 parts)
- `geology-template.md` - Main geological overview (~500-550 lines)
- `geological-feature-template.md` - Individual geological features (~200-450 lines)
- `geography-template.md` - Geographic documentation
- `evolutionary-era-template.md` - Deep time era documentation
- `flora-overview-template.md` - **Flora overview documentation (~400 lines)**
- `flora-species-template.md` - Plant species documentation (~250-400 lines, includes lead quote)
- `fauna-overview-template.md` - **Fauna overview documentation (~400 lines)**
- `fauna-species-template.md` - Animal species documentation (~250-400 lines, includes lead quote)
- `municipality-template.md` - City/town/county profiles
- `cultural-organization-template.md` - Governance documentation
- `human-history-era-template.md` - Historical period documentation
- `significant-figure-template.md` - Regional figure biography
- `significant-figure-short-bio-template.md` - Short biography
- `landmark-template.md` - Natural/cultural landmarks

### `/queries/`
Research query templates:
- `narrative-research-methodology.md` - Core methodology document
- `region-overview-query.md` - Comprehensive region research
- `geological-survey-query.md` - Geology and tectonics
- `geographical-analysis-query.md` - Climate, hydrology, topography
- `evolutionary-history-query.md` - Deep time and paleontology
- `flora-documentation-query.md` - Plant species research
- `fauna-documentation-query.md` - Animal species research
- `cultural-analysis-query.md` - Cultural/municipal research
- `human-history-query.md` - Archaeological to modern history
- `significant-figure-biography-query.md` - Regional figure biographies
- `extended-region-overview-query.md` - 10-part overview framework

### `/commentaries/templates/`
Templates for creating documentary episodes, podcast series, or educational content based on the core content database.

---

## Notes

This project follows a standardized organizational schema for documenting geographic regions. The structure supports comprehensive documentation of Taos, New Mexico's geology, geography, natural history, human history, and significant figures.

All content should be:
- **Fact-checked** and verified from reliable sources
- **Properly attributed** with source citations
- **Narratively weighted** to prioritize engaging content
- **Cross-referenced** between related documents

The narrative research methodology ensures that content is both academically rigorous and genuinely interesting to read.
