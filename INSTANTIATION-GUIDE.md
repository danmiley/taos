# Region Template Instantiation Guide

## Quick Start

This guide walks you through creating a new regional documentation project from this template.

---

## Step 1: Copy the Template

Copy the entire `region-template/` directory to a new location with a descriptive name:

```bash
cp -r region-template ../big-sur
# or
cp -r region-template ../yellowstone
# or
cp -r region-template ../patagonia
```

**Naming convention**: Use lowercase with hyphens (kebab-case).

---

## Step 2: Navigate to Your New Project

```bash
cd ../big-sur
```

---

## Step 3: Run the Instantiation Prompt

Open the project in Cursor and use one of these prompts:

### Basic Instantiation Prompt

```
Instantiate this region-template project for [YOUR REGION NAME].

Region Details:
- Region Name: [Full name]
- Region Type: [Coastal region, mountain range, national park, etc.]
- Location: [State/Country]
- Coordinates: [Approximate lat/long]

Primary Focus: [Choose: Geology, Natural History, Human History, Literary History, etc.]

Significant Figures: Focus on [4-8] [type of figures - literary, scientific, indigenous, political, etc.]

Actions:
1. Replace all [PLACEHOLDER] values in README.md with specific details
2. Update BOOTSTRAP-QUERIES.md with region-specific examples
3. Create initial overview draft in /drafts/overview/[region-name].md
4. Customize the biographies section for the specified figure type
```

### Example: Big Sur with Literary Figures

```
Instantiate this region-template project for Big Sur, California.

Region Details:
- Region Name: Big Sur
- Region Type: Coastal mountain wilderness
- Location: Monterey County, California, USA
- Coordinates: 36.2°N, 121.8°W
- Area: ~90 miles of coastline

Primary Focus: Literary History and Cultural Significance

Significant Figures: Focus on 6-8 literary figures, including:
- Henry Miller (writer, resident 1944-1962)
- Robinson Jeffers (poet, built Tor House)
- Jack Kerouac (wrote "Big Sur" novel)
- Hunter S. Thompson (worked at Big Sur Hot Springs)
- Richard Brautigan (frequented Big Sur)
- Lawrence Ferlinghetti (City Lights connection)
- Kim Stanley Robinson (contemporary author)
- Consider also: artists, photographers, musicians drawn to the region

Actions:
1. Replace all [PLACEHOLDER] values in README.md
2. Update BOOTSTRAP-QUERIES.md with Big Sur examples
3. Create initial overview draft in /drafts/overview/big-sur.md
4. Customize biographies section for literary/artistic figures
5. Note: Emphasize the Bohemian/Beat culture connection in human history
```

### Example: Yellowstone with Scientific Focus

```
Instantiate this region-template project for Yellowstone National Park.

Region Details:
- Region Name: Yellowstone National Park
- Region Type: National Park / Volcanic caldera
- Location: Wyoming, Montana, Idaho, USA
- Coordinates: 44.4°N, 110.5°W
- Area: 2.2 million acres

Primary Focus: Geology and Geothermal Features

Significant Figures: Focus on 6 figures including:
- John Colter (first European-American to explore)
- Ferdinand Hayden (led geological survey)
- Thomas Moran (painter whose work helped establish the park)
- Teddy Roosevelt (conservation president)
- George Bird Grinnell (conservationist)
- Modern research scientists

Actions:
1. Replace all [PLACEHOLDER] values in README.md
2. Update BOOTSTRAP-QUERIES.md with Yellowstone examples
3. Create initial overview draft in /drafts/overview/yellowstone.md
4. Customize for scientific/conservation figures
```

### Example: Cultural/Indigenous Focus

```
Instantiate this region-template project for Mesa Verde.

Region Details:
- Region Name: Mesa Verde
- Region Type: National Park / Archaeological site
- Location: Montezuma County, Colorado, USA
- Coordinates: 37.2°N, 108.5°W

Primary Focus: Human History and Archaeology

Significant Figures: Focus on 6-8 figures including:
- Ancestral Puebloan leaders (as known through oral history)
- Richard Wetherill (rancher who explored cliff dwellings)
- Gustaf Nordenskiöld (early archaeologist)
- Virginia McClurg (advocate for park creation)
- Modern Pueblo tribal leaders
- Contemporary archaeologists

Actions:
1. Replace all [PLACEHOLDER] values in README.md
2. Update BOOTSTRAP-QUERIES.md with Mesa Verde examples
3. Create initial overview draft in /drafts/overview/mesa-verde.md
4. Customize for archaeological/indigenous focus
5. Note: Emphasize respectful treatment of indigenous perspectives
```

---

## Step 4: Verify Placeholder Replacement

After running the instantiation prompt, verify these files were updated:

### Checklist

- [ ] **README.md** - All `[PLACEHOLDER]` values replaced
  - [ ] `[REGION-NAME]` → Your region name
  - [ ] `[REGION-CLASSIFICATION]` → Region type
  - [ ] `[LATITUDE]`, `[LONGITUDE]` → Coordinates
  - [ ] `[AREA]` → Size
  - [ ] `[BOUNDARY-DESCRIPTION]` → Boundaries
  - [ ] `[PRIMARY-DEEP-DIVE-TOPIC]` → Your focus area
  - [ ] `[DATE]` → Current date

- [ ] **BOOTSTRAP-QUERIES.md** - Placeholders replaced with examples
  - [ ] `[REGION-NAME]` throughout
  - [ ] Example figures listed
  - [ ] Example landmarks listed

- [ ] **Initial draft created** in `/drafts/overview/[region-name].md`

---

## Step 5: Customize the Biography Section

The template defaults to a general "significant figures" approach. For specialized focus:

### For Literary Figures
Consider adding to `templates/significant-figure-template.md`:
- Published works section
- Literary style and themes
- Influence on other writers
- Connection between place and writing

### For Scientific Figures
Consider adding:
- Major discoveries/contributions
- Institutional affiliations
- Published research
- Scientific legacy

### For Indigenous Leaders
Consider adding:
- Tribal affiliation
- Traditional role
- Oral history sources
- Living descendants/legacy keepers
- Cultural sensitivity notes

---

## Step 6: Begin Content Creation

Use the phased approach from `BOOTSTRAP-QUERIES.md`:

### Recommended Order

1. **Short Overview** → `/drafts/overview/[region-name].md`
2. **Geography** → `/drafts/geography/`
3. **Geology** (if relevant) → `/drafts/geology/`
4. **Natural History** → `/drafts/natural-history/`
5. **Human History** → `/drafts/human-history/`
6. **Cultural Organization** → `/drafts/cultural-organization/`
7. **Significant Figures** → `/drafts/biographies/`
8. **Extended Overview** (10 parts) → `/drafts/overview/`

### For Each Section

Use the corresponding query template from `/queries/`:
- `region-overview-query.md`
- `geological-survey-query.md`
- `geographical-analysis-query.md`
- `evolutionary-history-query.md` — **Note: Uses three-document structure**
- `flora-documentation-query.md`
- `fauna-documentation-query.md`
- `human-history-query.md`
- `cultural-analysis-query.md`
- `significant-figure-biography-query.md`

### Evolutionary History Special Note

Evolutionary history uses a **three-document structure** (~950-1,100 total lines):

| Document | Lines | Focus |
|----------|-------|-------|
| `[region]-deep-time.md` | ~400-450 | Main comprehensive overview |
| `cenozoic-era.md` | ~300-350 | Age of Mammals; glaciation |
| `fossil-record.md` | ~250-300 | Paleontology; proxy records |

For fossil-poor regions (granite, metamorphic, heavily eroded), frame the absence as the story:
- "The Granite Problem"
- "The Glacial Erasure"
- "The Metamorphic Gap"

Include proxy records (tree rings, lake cores, pollen) and living fossils.

---

## Customization Options

### Changing the Biography Focus

The template includes a generic "significant figures" section. To specialize:

**Option A**: Rename the section in documentation
- Change "Significant Figures" to "Literary Figures" or "Scientific Pioneers" etc.

**Option B**: Create specialized templates
- Copy `significant-figure-template.md`
- Rename to `literary-figure-template.md`
- Add fields specific to writers (bibliography, literary movements, etc.)

**Option C**: Add specialized query
- Copy `significant-figure-biography-query.md`
- Rename to `literary-figure-biography-query.md`
- Customize research prompts for literary context

### Adding Region-Specific Sections

If your region needs specialized sections not in the template:

1. Create new directory in `/docs/` and `/drafts/`
2. Create template in `/templates/`
3. Create query in `/queries/`
4. Update `project-schema.md` to document

**Examples**:
- Big Sur → Add `/docs/literary-history/` section
- Yellowstone → Add `/docs/geothermal-features/` section
- Mesa Verde → Add `/docs/archaeology/` section

---

## Narrative Weighting Reminder

Remember to apply narrative weighting throughout all content:

| Flag | What to Look For |
|------|------------------|
| `[UNEXPECTED]` | Facts that surprise or contradict assumptions |
| `[PARADOX]` | Apparent contradictions that can be explained |
| `[UNUSUAL]` | Rare features, statistical outliers, firsts |
| `[HUMAN]` | Personal stories, character-revealing moments |
| `[TURNING]` | Pivotal moments, near-misses, what-ifs |

**Goal**: Create content that makes readers say "I never knew that!" while maintaining factual accuracy.

---

## Quick Reference: File Locations

| Purpose | Location |
|---------|----------|
| Main documentation | `README.md` |
| Research queries | `/queries/` |
| Document templates | `/templates/` |
| Work in progress | `/drafts/` |
| Vetted content | `/docs/` |
| Source materials | `/library/` |
| New/unsorted materials | `/research/` |
| Derivative content | `/commentaries/` |
| Schema documentation | `/bootstrap-instructions/` |

---

## Troubleshooting

### "Placeholders still showing"
Run a search for remaining placeholders:
```bash
grep -r "\[REGION-NAME\]" .
grep -r "\[PLACEHOLDER\]" .
```

### "Directory structure seems wrong"
Verify against the schema:
```bash
cat bootstrap-instructions/project-schema.md
```

### "Not sure which query to use"
Check the query index in `BOOTSTRAP-QUERIES.md` - it lists all queries in recommended order.

### "Need to add a section not in template"
Follow the customization instructions above, or create an issue/request for future template versions.

---

## Example: Complete Big Sur Instantiation

Here's a complete example session:

```bash
# 1. Copy template
cp -r region-template ../big-sur
cd ../big-sur

# 2. Open in Cursor and run instantiation prompt (see above)

# 3. Verify files updated
grep "Big Sur" README.md  # Should show replacements

# 4. Start content creation
# Use queries/region-overview-query.md to create:
# /drafts/overview/big-sur.md

# 5. Work through sections...
```

---

## Getting Help

- **Schema questions**: See `bootstrap-instructions/project-schema.md`
- **Query guidance**: See `queries/narrative-research-methodology.md`
- **Template formats**: See individual files in `/templates/`
- **Phased workflow**: See `BOOTSTRAP-QUERIES.md`

---

*Instantiation Guide v1.0 - November 2025*





