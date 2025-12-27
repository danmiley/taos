# Bootstrap Queries for Taos, New Mexico Regional Concordance

## Overview

This document provides ready-to-use prompts for generating content in the Taos, New Mexico regional concordance project. All queries incorporate **narrative-weighted research methodology** to produce engaging, memorable content.

### Narrative Weighting Reminder

Apply these criteria throughout all research:

| Flag | Criterion | Look For |
|------|-----------|----------|
| `[UNEXPECTED]` | The Unexpected | Facts contradicting common assumptions |
| `[PARADOX]` | Paradox Resolution | Details reconciling conflicting accounts |
| `[UNUSUAL]` | The Unusual | Outliers, anomalies, statistical rarities |
| `[HUMAN]` | Human Interest | Personal stories, character-revealing details |
| `[TURNING]` | Turning Points | Moments where outcomes hung in balance |

See `queries/narrative-research-methodology.md` for complete methodology.

---

## Phase 1: Foundation - Regional Overview

### Two-Tier Overview System

| Type | File | Lines | Purpose |
|------|------|-------|---------|
| **Short Overview** | `taos.md` | ~100-150 | Quick reference |
| **Extended Overview** | `taos-extended-overview-part-[1-10].md` | ~1000+ | Comprehensive (10 parts) |

---

### Phase 1A: Short Overview

**Template**: `templates/region-short-overview-template.md`

**Prompt**:
```
Create a short overview (~100-150 lines) for Taos, New Mexico using the 
region-short-overview-template.md format.

Include:
- Basic information table (coordinates, area, boundaries, climate)
- Geographic summary (2-3 paragraphs)
- Quick facts highlighting narrative-weight content
- Key statistics and notable features
- Links to extended documentation

Apply narrative weighting: Flag all [UNEXPECTED], [UNUSUAL], or [TURNING] 
content prominently.
```

**Target**: `/drafts/overview/taos.md`

---

### Phase 1B: Extended Overview (10 Parts)

**Template**: `templates/region-extended-overview-template.md`
**Query Guide**: `queries/extended-region-overview-query.md`

**Strategy**: Create in 10 separate files with timestamp checkpoints for resilience.

#### Part Structure

| Part | Prompt | Sections |
|------|--------|----------|
| 1 | Basic Info, Geographic Overview, Boundaries | I-II |
| 2 | Geological Foundation, Tectonic History | III-IV |
| 3 | Geography: Topography, Climate, Hydrology | V-VII |
| 4 | Evolutionary History, Paleontology | VIII-IX |
| 5 | Natural History: Flora Overview | X-XI |
| 6 | Natural History: Fauna Overview | XII-XIII |
| 7 | Human History: Prehistory to Colonial Era | XIV-XVI |
| 8 | Human History: Modern Era to Present | XVII-XIX |
| 9 | Cultural Organization, Demographics | XX-XXII |
| 10 | Significant Figures, Legacy, Sources | XXIII-XXV |

#### Extended Overview Part Prompt Template

```
Create Part [X] of the extended overview for Taos, New Mexico.

**File**: `taos-extended-overview-part-[X].md`

**Sections to cover**:
[List sections from table above]

**Requirements**:
- ~100 lines of detailed content
- Use YAML frontmatter with: part: [X], total_parts: 10
- Apply narrative weighting throughout
- Flag all [UNEXPECTED], [PARADOX], [UNUSUAL], [HUMAN], [TURNING] content
- End with timestamp: *Part [X] completed at [YYYY-MM-DDTHH:MM:SSZ]*
- Include navigation link to Part [X+1]
```

**Targets**: `/drafts/overview/taos-extended-overview-part-[1-10].md`

---

## Phase 2: Geology Deep Dive

### 2.1 Geological Overview

**Template**: `templates/geology-template.md`
**Query**: `queries/geological-survey-query.md`

**Prompt**:
```
Create comprehensive geological documentation for Taos, New Mexico including:

- Tectonic setting and plate history
- Major rock formations and stratigraphy
- Geological timeline (Precambrian to present)
- Mineral resources and economic geology
- Soil composition and distribution
- Geological hazards (earthquakes, volcanism, landslides)
- Notable geological features and formations

Apply narrative weighting:
- Flag catastrophic events as [TURNING]
- Flag unusual formations as [UNUSUAL]
- Flag discovery stories as [HUMAN]
- Flag counter-intuitive facts as [UNEXPECTED]
```

**Target**: `/drafts/geology/taos-geology.md`

---

### 2.2 Individual Geological Features

For each major geological feature:

**Prompt**:
```
Document [GEOLOGICAL-FEATURE-NAME] in Taos, New Mexico:

- Formation process and geological age
- Composition and structure
- Unique characteristics [UNUSUAL]
- Discovery history [HUMAN]
- Scientific significance
- Current status and any threats
- Visitor/research access

What makes this feature narratively compelling?
```

**Target**: `/drafts/geology/[feature-name].md`

---

## Phase 3: Geography Documentation

### 3.1 Geographic Overview

**Template**: `templates/geography-template.md`
**Query**: `queries/geographical-analysis-query.md`

**Prompt**:
```
Document the geography of Taos, New Mexico including:

**Topography**:
- Elevation ranges and major landforms
- Mountain systems and peaks
- Valleys, plains, and plateaus
- Coastal features (if applicable)

**Climate**:
- Climate classification
- Temperature ranges (seasonal)
- Precipitation patterns
- Extreme weather events [UNUSUAL] [TURNING]
- Microclimates [UNEXPECTED]

**Hydrology**:
- Major rivers and their courses
- Lakes and reservoirs
- Groundwater systems
- Wetlands and marshes
- Historical changes to waterways [TURNING]

**Ecosystems**:
- Biome classification
- Vegetation zones
- Habitat types
- Ecological transitions

Apply narrative weighting throughout.
```

**Target**: `/drafts/geography/taos-geography.md`

---

## Phase 4: Evolutionary History

### 4.1 Deep Time Overview

**Template**: `templates/evolutionary-era-template.md`
**Query**: `queries/evolutionary-history-query.md`

**Prompt**:
```
Document the evolutionary history of Taos, New Mexico through deep time:

**Precambrian** (4.6 BYA - 538 MYA):
- Earliest geological record
- Formation of basement rocks

**Paleozoic** (538 - 252 MYA):
- Marine environments and life
- Transition to terrestrial ecosystems
- Permian extinction impact [TURNING]

**Mesozoic** (252 - 66 MYA):
- Dinosaur presence and fossil record
- Flora during the era
- K-Pg extinction impact [TURNING]

**Cenozoic** (66 MYA - present):
- Mammalian radiation
- Development of modern ecosystems
- Ice age impacts [TURNING]
- Human arrival [TURNING]

For each era, prioritize:
- [UNUSUAL] species or adaptations
- [UNEXPECTED] fossil discoveries
- [TURNING] extinction or climate events
- [HUMAN] stories of scientific discovery
```

**Target**: `/drafts/evolutionary-history/taos-deep-time.md`

---

## Phase 5: Natural History

Natural history documentation uses a structured approach with overview documents and individual species profiles. Each species profile opens with a **biographical lead quote** from a project figure.

### 5.0 Natural History Planning

Before creating documents, plan your coverage:

#### Flora Target Structure

| Document Type | Count | Lines Each | Total Lines |
|---------------|-------|------------|-------------|
| Flora Overview | 1 | ~400 | ~400 |
| High-Profile Flora | 2-3 | ~350-400 | ~700-1,200 |
| Standard Flora | 3-5 | ~250-300 | ~750-1,500 |
| **Flora Total** | **6-9** | — | **~1,850-3,100** |

#### Fauna Target Structure

| Document Type | Count | Lines Each | Total Lines |
|---------------|-------|------------|-------------|
| Fauna Overview | 1 | ~400 | ~400 |
| High-Profile Fauna | 3-4 | ~350-400 | ~1,050-1,600 |
| Standard Fauna | 5-8 | ~250-300 | ~1,250-2,400 |
| **Fauna Total** | **9-13** | — | **~2,700-4,400** |

#### Combined Natural History Output

**Total: 15-22 documents, ~4,550-7,500 lines**

### 5.1 Biographical Lead Quote Research

**Before creating species profiles**, research quotes from project biographical figures:

**Prompt**:
```
Research quotes from Taos, New Mexico biographical figures for flora and fauna lead quotes.

Search for quotes from each figure in /docs/biographies/ mentioning:
- Specific plant or animal species
- Ecosystems, habitats, or vegetation types
- Wildlife encounters or observations
- General reflections on nature, wilderness, or ecological themes

For each figure, compile a quote bank organized by:
1. Species-specific quotes (highest priority)
2. Habitat/ecosystem quotes
3. General nature quotes

Include full citations: author, source work, year, page if available.
```

**Target**: Keep notes for reference during species documentation

---

### 5.2 Flora Overview

**Template**: `templates/flora-overview-template.md`
**Query**: `queries/flora-documentation-query.md`

**Prompt**:
```
Create a comprehensive flora overview for Taos, New Mexico (~400 lines):

**Structure**:
- Basic Information table (species count, vegetation types, endemics)
- Narrative Highlights table with `[UNEXPECTED]`, `[UNUSUAL]`, `[TURNING]`, `[HUMAN]` flags
- Introduction and ecological context
- Major plant communities/vegetation zones
- Endemic and notable species table (linking to individual profiles)
- Conservation status summary
- Indigenous ethnobotany overview `[HUMAN]`
- Seasonal patterns and phenology
- Research history
- Cross-references to species profiles

Apply narrative weighting throughout. Flag all compelling content.
```

**Target**: `/drafts/natural-history/flora/taos-flora-overview.md`

---

### 5.3 Flora Species Profiles

**Template**: `templates/flora-species-template.md`
**Query**: `queries/flora-documentation-query.md`

#### Species Selection Criteria

| Priority | Criterion | Example |
|----------|-----------|---------|
| 1 | Endemic/regional specialty | Found only here |
| 2 | Conservation story | Threatened or recovering `[TURNING]` |
| 3 | Indigenous connection | Traditional use documented `[HUMAN]` |
| 4 | Ecological keystone | Shapes the ecosystem |
| 5 | Climate indicator | Sensitive to environmental change |
| 6 | Visitor recognition | Flagship species |

#### Species Prompt Template

```
Create a species profile for [SPECIES-NAME] in Taos, New Mexico:

**Biographical Lead Quote**: 
Open with an inspiring quote from [FIGURE-NAME] about this species or its habitat.
Format: > "Quote" — **Name**, *Source* (Year)

**Target Length**: [~350-400 for high-profile / ~250-300 for standard]

**Narrative Focus**: [PRIMARY-FLAG, e.g., [TURNING] for conservation story]

**Include**:
- Basic Information table
- Narrative Highlights table
- Physical description with identifying features
- Ecology and habitat
- Distribution in Taos, New Mexico
- Conservation status and history
- Cultural significance `[HUMAN]`
- Research and discovery history
- Where/when to observe
- Cross-references

Apply narrative weighting. Prioritize engaging content.
```

**Targets**: `/drafts/natural-history/flora/[species-name].md`

---

### 5.4 Fauna Overview

**Template**: `templates/fauna-overview-template.md`
**Query**: `queries/fauna-documentation-query.md`

**Prompt**:
```
Create a comprehensive fauna overview for Taos, New Mexico (~400 lines):

**Structure**:
- Basic Information table (species counts by class, endemics, threatened)
- Narrative Highlights table with `[UNEXPECTED]`, `[UNUSUAL]`, `[TURNING]`, `[HUMAN]` flags
- Introduction and ecological context
- Mammals summary
- Birds summary
- Reptiles and amphibians summary
- Fish and aquatic species summary (if applicable)
- Endemic and notable species table (linking to individual profiles)
- Conservation status summary
- Human-wildlife interactions overview
- Indigenous connections `[HUMAN]`
- Research history
- Cross-references to species profiles

Apply narrative weighting throughout. Flag all compelling content.
```

**Target**: `/drafts/natural-history/fauna/taos-fauna-overview.md`

---

### 5.5 Fauna Species Profiles

**Template**: `templates/fauna-species-template.md`
**Query**: `queries/fauna-documentation-query.md`

#### Species Selection Criteria

| Priority | Criterion | Example |
|----------|-----------|---------|
| 1 | Endemic subspecies | Unique to region |
| 2 | Conservation milestone | Recovery or extinction story `[TURNING]` |
| 3 | Keystone predator/herbivore | Shapes ecosystem dynamics |
| 4 | Indigenous significance | Cultural importance `[HUMAN]` |
| 5 | Human-wildlife interface | Notable interactions |
| 6 | Climate sentinel | Indicator species |
| 7 | Charismatic megafauna | Visitor draw |

#### Taxonomic Balance Guide

| Group | Target Count | Selection Focus |
|-------|--------------|-----------------|
| Mammals | 3-5 | Include predator, large herbivore, small mammal |
| Birds | 2-4 | Include raptor, songbird, or specialty |
| Fish | 1-2 | Native aquatic species (if applicable) |
| Other | 0-2 | Regionally iconic reptiles, amphibians, invertebrates |

#### Species Prompt Template

```
Create a species profile for [SPECIES-NAME] in Taos, New Mexico:

**Biographical Lead Quote**: 
Open with an inspiring quote from [FIGURE-NAME] about this species or wildlife.
Format: > "Quote" — **Name**, *Source* (Year)

**Target Length**: [~350-400 for high-profile / ~250-300 for standard]

**Narrative Focus**: [PRIMARY-FLAG, e.g., [TURNING] for conservation story]

**Include**:
- Basic Information table
- Narrative Highlights table
- Physical description with identifying features
- Behavior and ecology
- Distribution in Taos, New Mexico
- Conservation status and history `[TURNING]`
- Human interactions
- Cultural significance `[HUMAN]`
- Research and discovery history
- Where/when to observe
- Safety considerations (if applicable)
- Cross-references

Apply narrative weighting. Prioritize engaging content.
```

**Targets**: `/drafts/natural-history/fauna/[species-name].md`

---

### 5.6 Natural History Execution Order

**Recommended sequence**:

1. Research biographical quotes for lead quote bank
2. Create flora overview
3. Create fauna overview
4. Create high-profile flora species (2-3 documents)
5. Create high-profile fauna species (3-4 documents)
6. Create standard flora species (3-5 documents)
7. Create standard fauna species (5-8 documents)
8. Update overviews with cross-references

**Checkpoint**: After completing natural history, you should have:
- 2 overview documents (~800 lines)
- 6-8 flora profiles (~1,700-2,600 lines)
- 8-12 fauna profiles (~2,400-4,000 lines)
- **Total: ~16-22 documents, ~4,900-7,400 lines**

---

## Phase 6: Human History

### 6.1 Comprehensive History

**Template**: `templates/human-history-era-template.md`
**Query**: `queries/human-history-query.md`

**Prompt**:
```
Document the human history of Taos, New Mexico:

**Prehistory**:
- First human presence [TURNING]
- Archaeological sites and findings
- Indigenous peoples and cultures
- Pre-contact lifeways

**Early History**:
- First written records
- Indigenous governance systems
- Trade networks and connections
- Early conflicts and alliances [TURNING]

**Colonial/Contact Period**:
- First external contact [TURNING]
- Colonial powers and claims
- Impact on indigenous peoples [TURNING]
- Resistance and adaptation [HUMAN]

**Modern History**:
- Political developments [TURNING]
- Economic transformations
- Social changes
- Environmental impacts

**Contemporary Era**:
- Current governance
- Recent developments
- Ongoing issues and challenges
- Future prospects

Prioritize:
- [TURNING] points that shaped the region
- [HUMAN] stories of individuals who made a difference
- [UNEXPECTED] facts that challenge assumptions
- [PARADOX] elements that explain apparent contradictions
```

**Target**: `/drafts/human-history/taos-history.md`

---

### 6.2 Historical Era Documentation

For major historical periods:

**Prompt**:
```
Document [ERA-NAME] in Taos, New Mexico ([DATE-RANGE]):

- Key events and developments
- Major figures [HUMAN]
- Social and economic conditions
- Cultural developments
- Environmental changes
- Turning points [TURNING]
- Legacy and lasting impacts

What nearly happened differently? [TURNING]
What surprises people about this era? [UNEXPECTED]
```

**Target**: `/drafts/human-history/[era-name].md`

---

## Phase 7: Cultural Organization

### 7.1 Cultural Overview

**Template**: `templates/cultural-organization-template.md`
**Query**: `queries/cultural-analysis-query.md`

**Prompt**:
```
Document the current cultural organization of Taos, New Mexico:

**Governance**:
- Political structure and jurisdiction
- Administrative divisions
- Relationship to larger political entities
- Unique governance features [UNUSUAL]

**Demographics**:
- Population statistics
- Ethnic and cultural composition
- Languages spoken
- Religious affiliations
- Population trends [TURNING]

**Economy**:
- Major economic sectors
- Key industries
- Employment patterns
- Economic challenges and opportunities

**Infrastructure**:
- Transportation networks
- Utilities and services
- Communications
- Healthcare and education

**Cultural Institutions**:
- Museums and cultural centers
- Educational institutions
- Religious sites
- Community organizations

Flag:
- [UNEXPECTED] demographic shifts
- [UNUSUAL] governance arrangements
- [TURNING] economic transformations
- [PARADOX] cultural tensions or reconciliations
```

**Target**: `/drafts/cultural-organization/taos-cultural-overview.md`

---

### 7.2 Municipality Profiles

**Template**: `templates/municipality-template.md`

For major cities, towns, or administrative units:

**Prompt**:
```
Create a profile for [MUNICIPALITY-NAME] in Taos, New Mexico:

- Location and boundaries
- Population and demographics
- History and founding [TURNING]
- Economic base
- Notable features and landmarks
- Cultural significance
- Challenges and opportunities
- Interesting facts [UNEXPECTED] [UNUSUAL]
```

**Target**: `/drafts/cultural-organization/municipalities/[municipality-name].md`

---

## Phase 8: Significant Figures (4-8 Biographies)

### 8.1 Figure Selection

Identify 4-8 historically significant figures representing:
- Indigenous leaders
- Explorers/scientists
- Political figures
- Cultural icons
- Conservationists
- Other regionally significant individuals

### 8.2 Biography Documentation

**Template**: `templates/significant-figure-template.md`
**Query**: `queries/significant-figure-biography-query.md`

**CRITICAL REQUIREMENT**: Every biography must include a **"Taos, New Mexico Record"** section immediately after the Basic Information table. This section consolidates all dated, specific information about the figure's connection to the region.

**Prompt**:
```
Create a biography for [FIGURE-NAME], significant to Taos, New Mexico:

**Basic Information**:
- Full name and life dates
- Role/profession
- Connection to Taos, New Mexico

**Taos, New Mexico Record** (REQUIRED - place after Basic Information):
- First arrival date and circumstances
- Total time in region (with date range)
- Residency type (permanent/extended visits/brief visits)
- Primary location within region
- Chronology of visits/residency with dated events
- Works created or related to the region (titles with dates)
- Significant activities during time in region (with dates)
- Notable encounters with other significant figures (with dates and context)

**Life Story**:
- Early life and background
- How they came to Taos, New Mexico or their origins there
- Major contributions or actions
- Character-revealing moments [HUMAN]
- Challenges and setbacks
- Legacy and lasting impact

**Narrative Focus**:
- What makes their story compelling? [HUMAN]
- What would surprise people about them? [UNEXPECTED]
- What turning points defined their life? [TURNING]
- What contradictions or paradoxes exist? [PARADOX]

**Connection to Region**:
- How they shaped Taos, New Mexico
- Physical traces they left (buildings, landmarks, etc.)
- How they are remembered today

**Encounters Research**:
- Who else of significance did they meet in the region?
- Are there documented interactions with other figures in this project?
- What anecdotes exist about meetings between significant figures?
```

**Target**: `/drafts/biographies/[figure-name].md`

---

### 8.3 Taos, New Mexico Record Guidelines

The **Taos, New Mexico Record** section ensures every biography answers these questions with specific dates:

| Question | Subsection |
|----------|------------|
| When did they first arrive? | Arrival and Residency |
| How long were they there? | Arrival and Residency |
| What is the dated chronology of their time there? | Chronology |
| What did they create there or about the region? | Works Created |
| What significant things did they do there? | Significant Activities |
| Who else of importance did they encounter there? | Notable Encounters |

This section enables:
- **Timeline integration**: Easy extraction of dates for regional timeline
- **Cross-referencing**: Linking encounters between documented figures
- **Quick reference**: Immediate access to regional connection facts
- **Verification**: Clear dates make fact-checking straightforward

---

### 8.3 Short Biography Format

**Template**: `templates/significant-figure-short-bio-template.md`

**Prompt**:
```
Create a short biography (~100 lines) for [FIGURE-NAME]:

- Basic information table
- Summary biography (3-4 paragraphs)
- Key achievements
- Connection to Taos, New Mexico
- Legacy
- One compelling [HUMAN] or [UNEXPECTED] detail
```

**Target**: `/drafts/biographies/[figure-name]-short.md`

---

## Phase 9: Landmarks

### 9.1 Natural Landmarks

**Template**: `templates/landmark-template.md`

**Prompt**:
```
Document [LANDMARK-NAME], a natural landmark in Taos, New Mexico:

- Location and access
- Physical description
- Geological/ecological significance
- Formation history [UNUSUAL]
- Cultural significance [HUMAN]
- Discovery or naming history
- Conservation status
- Visitor information
```

**Target**: `/drafts/landmarks/[landmark-name].md`

---

### 9.2 Cultural/Historical Landmarks

**Prompt**:
```
Document [LANDMARK-NAME], a cultural landmark in Taos, New Mexico:

- Location and access
- Physical description
- Historical significance [TURNING]
- Construction/creation history [HUMAN]
- Cultural importance
- Current status and preservation
- Notable events that occurred here [TURNING]
- Visitor information
```

**Target**: `/drafts/landmarks/[landmark-name].md`

---

## Phase 10: Essays (Long-Form Interpretive Content)

Essays complement documentary content with narrative-driven explorations. They follow principles from Rebecca Solnit (lateral thinking, spiraling from specific to universal) and John McPhee (geological patience, deep time).

**Templates**: `templates/essay-template.md`
**Query Guide**: `queries/essay-development-query.md`
**Planning Doc**: `docs/essays/ESSAY-PLANNING.md`
**Index**: `docs/essays/README.md`

### 10.1 Essay Development Process

**Target Length**: 4,000-6,000 words per essay

**Key Requirements**:
- Begin with specific object/place/fact, spiral outward
- Seek counterintuitive arguments grounded in evidence
- Honor specificity (names, dates, species)
- End with open questions, not closed conclusions
- Include annotated bibliography for general readers

**CRITICAL**: Human review required between each essay. Do not begin Essay N+1 until Essay N is approved.

### 10.2 Essay Categories

| Category | Focus | Examples |
|----------|-------|----------|
| **History** | Human past through unexpected angles | Infrastructure paradoxes, failed projects, hermit sequences |
| **Themes** | Ecology, geology, culture explorations | Natural phenomena as protagonists, species biographies |
| **Perspectives** | Comparative and philosophical | Regional comparisons, landscape philosophy |

### 10.3 Essay Prompt Template

```
Write Essay [N]: "[TITLE]" for the Taos, New Mexico Essays series.

**Category**: [History/Themes/Perspectives]
**Target File**: `drafts/essays/[category]/[NN]-[slug].md`

**Starting Point**: [Specific object, place, or fact to begin with]

**The Spiral**: [What larger questions does this lead to?]

**The Twist**: [Counterintuitive argument]

**Requirements**:
- Target 4,000-6,000 words
- Follow Solnit/McPhee methodology
- Apply narrative weighting flags
- Include annotated bibliography (5-10 sources)
- Cross-reference project documentation
- End with open question

**Project Cross-References to Draw From**:
- [List relevant docs]
```

### 10.4 Example Essay Types

**Infrastructure Paradox**: How [project] intended to do X actually accomplished the opposite.

**Species Biography**: [Species] story across three timescales (deep time, historical, modern).

**Hermit Sequence**: Succession of [type of people] who used region's isolation for specific purposes.

**Fire/Climate Regime**: Three eras—indigenous management, suppression, transformed return.

**Geological Siblings**: Region in conversation with similar landscapes globally.

**Atmospheric Protagonist**: Natural phenomenon (fog, fire, tides) as active agent.

**Failure Archive**: Projects that didn't happen and how refusal shaped regional character.

### 10.5 Human Review Workflow

```
Draft Essay → Human Review → Approved? → Promote to docs/essays/ → Begin Next
                    ↓
                 Revise
```

**Review Criteria**:
- Accuracy (facts verified)
- Argument (counterintuitive but grounded)
- Tone (patient, specific, spiraling)
- Bibliography (accessible, annotated)
- Length (4,000-6,000 words)

---

## Additional Content Development

### Complete Timeline

**Prompt**:
```
Create a comprehensive timeline for Taos, New Mexico from geological formation 
to present:

**Geological Timeline** (billions to millions of years):
- Formation events
- Major geological changes [TURNING]

**Evolutionary Timeline** (millions of years):
- Key fossil appearances
- Extinction events [TURNING]

**Human Timeline** (thousands of years to present):
- First human presence
- Major historical events [TURNING]
- Modern developments

Highlight all [TURNING] points prominently.
```

**Target**: `/drafts/timeline/taos-timeline.md`

---

## Query Execution Order

### Recommended Sequence:

1. **START**: Regional short overview (Phase 1A)
2. Extended overview Part 1-2 (basic info, geology)
3. Geology deep dive (Phase 2)
4. Geography documentation (Phase 3)
5. Extended overview Part 3-4 (geography, evolution)
6. Evolutionary history (Phase 4)
7. Extended overview Part 5-6 (natural history)
8. Flora documentation (Phase 5.1)
9. Fauna documentation (Phase 5.2)
10. Extended overview Part 7-8 (human history)
11. Human history (Phase 6)
12. Extended overview Part 9 (cultural organization)
13. Cultural organization (Phase 7)
14. Extended overview Part 10 (significant figures)
15. Significant figure biographies (Phase 8)
16. Landmarks (Phase 9)
17. Complete timeline
18. **Essays (Phase 10)**: Long-form interpretive content (8-12 essays)

### Estimated Output:
- 1 short overview (~150 lines)
- 10 extended overview parts (~1000 lines total)
- 1 geology document (~500 lines)
- 1 geography document (~500 lines)
- 1 evolutionary history document (~500 lines)
- **1 flora overview (~400 lines)**
- **6-8 flora species profiles (~1,700-2,600 lines total)**
- **1 fauna overview (~400 lines)**
- **8-12 fauna species profiles (~2,400-4,000 lines total)**
- 1 human history document (~800 lines)
- 3+ historical era documents (~300 lines each)
- 1 cultural overview (~400 lines)
- 3+ municipality profiles (~150 lines each)
- 4-8 significant figure biographies (~400 lines each)
- 5+ landmark documents (~200 lines each)
- 1 timeline (~300 lines)
- 8-12 long-form essays (~4,000-6,000 words each)

**Natural History Subtotal: 16-22 documents, ~4,900-7,400 lines**

**Total: 60,000+ words of narrative-weighted regional content**

---

## Tips for Using These Queries

1. **Copy-paste prompts** directly into your AI assistant
2. **Apply narrative weighting** consistently—flag all compelling content
3. **Customize with specific details** as you discover them
4. **Add sources** to `/library/` before or during content generation
5. **Use multiple passes** - generate initial content, then refine
6. **Cross-reference** between documents as you build the database
7. **Verify facts** from multiple sources before moving to `/docs/`
8. **Maintain consistent formatting** using the templates

---

## Success Criteria

Regional documentation is complete when you have:

- ✅ Short overview with key facts and narrative highlights
- ✅ Extended 10-part overview with comprehensive coverage
- ✅ Geology documentation with formations and history
- ✅ Geography documentation with climate and hydrology
- ✅ Evolutionary history from deep time to present
- ✅ **Flora overview (~400 lines) covering vegetation zones and notable species**
- ✅ **6-8 flora species profiles with biographical lead quotes**
- ✅ **Fauna overview (~400 lines) covering wildlife groups and conservation**
- ✅ **8-12 fauna species profiles with biographical lead quotes**
- ✅ Human history from prehistory to present
- ✅ Cultural organization and demographics
- ✅ 4-8 significant figure biographies
- ✅ Landmark documentation (natural and cultural)
- ✅ Comprehensive timeline
- ✅ 8-12 long-form essays (Solnit/McPhee style)
- ✅ All content moved from `/drafts/` to `/docs/` after verification
- ✅ Narrative weighting applied throughout
- ✅ Complete cross-referencing between documents
- ✅ **All species profiles include biographical lead quotes from project figures**

---

*This bootstrap queries document provides everything needed to generate comprehensive regional documentation for the Taos, New Mexico concordance project.*
