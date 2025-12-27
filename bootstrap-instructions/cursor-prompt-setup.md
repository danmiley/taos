# Cursor Project Setup Prompt

## Purpose

This document provides step-by-step instructions for cursor.ai to set up a new geographic region project following the schema defined in `project-schema.md`.

-----

## Trigger Phrases

When the user says any of the following, execute the setup workflow:

- "Set up a new project for [Region Name]"
- "Create a region project for [Region Name]"
- "Initialize [Region Name] project"
- "Set up [Region Name]"
- "New region project: [Region Name]"

-----

## Setup Workflow

### Step 1: Gather Information

Ask the user for the following information:

1. **Region Name**: Full name of the geographic region
2. **Region Type**: (National park, river valley, mountain range, coastal region, urban area, historical territory, etc.)
3. **Geographic Location**: Approximate coordinates and/or country/state location
4. **Primary Deep Dive Topic**: Which section should receive special focus?
   - Geology
   - Natural History
   - Human History
   - Other
5. **Optional: Number of Significant Figures**: How many biographies (4-8 recommended)

-----

### Step 2: Create Top-Level Directory Structure

The following directories should already exist from the template. Verify they are present:

```bash
ls -la docs/ drafts/ library/ research/ commentaries/ templates/ queries/ bootstrap-instructions/
```

If any are missing, create them:

```bash
mkdir -p docs drafts library research commentaries templates queries bootstrap-instructions
```

-----

### Step 3: Verify `/docs/` Subdirectories

Ensure these subdirectories exist in `/docs/`:

```bash
mkdir -p docs/overview
mkdir -p docs/geology
mkdir -p docs/geography
mkdir -p docs/evolutionary-history
mkdir -p docs/natural-history/flora
mkdir -p docs/natural-history/fauna
mkdir -p docs/cultural-organization/municipalities
mkdir -p docs/human-history
mkdir -p docs/biographies
mkdir -p docs/landmarks
mkdir -p docs/timeline
mkdir -p docs/influences
mkdir -p docs/media/maps
mkdir -p docs/media/photos
mkdir -p docs/media/documentaries
mkdir -p docs/media/videos
```

-----

### Step 4: Verify `/drafts/` Mirror Structure

Mirror the same structure in `/drafts/`:

```bash
mkdir -p drafts/overview
mkdir -p drafts/geology
mkdir -p drafts/geography
mkdir -p drafts/evolutionary-history
mkdir -p drafts/natural-history/flora
mkdir -p drafts/natural-history/fauna
mkdir -p drafts/cultural-organization/municipalities
mkdir -p drafts/human-history
mkdir -p drafts/biographies
mkdir -p drafts/landmarks
mkdir -p drafts/timeline
mkdir -p drafts/influences
mkdir -p drafts/media/maps
mkdir -p drafts/media/photos
mkdir -p drafts/media/documentaries
mkdir -p drafts/media/videos
```

-----

### Step 5: Verify `/library/` Subdirectories

Ensure reference library structure exists:

```bash
mkdir -p library/academic
mkdir -p library/articles
mkdir -p library/books
mkdir -p library/essays
mkdir -p library/geological-surveys
mkdir -p library/maps
mkdir -p library/archaeological-records
mkdir -p library/municipal-records
mkdir -p library/natural-surveys
mkdir -p library/historical-documents
mkdir -p library/primary-sources
mkdir -p library/government-announcements
mkdir -p library/interviews
```

-----

### Step 6: Update Project README

Edit `README.md` to replace all placeholders with region-specific information:

| Placeholder | Replace With |
|-------------|--------------|
| `[REGION-NAME]` | Region name |
| `[REGION-CLASSIFICATION]` | Region type |
| `[LATITUDE]` | Latitude coordinate |
| `[LONGITUDE]` | Longitude coordinate |
| `[AREA]` | Size in sq km/sq miles |
| `[BOUNDARY-DESCRIPTION]` | Description of boundaries |
| `[PRIMARY-DEEP-DIVE-TOPIC]` | Main focus topic |
| `[PRIMARY-TOPIC]` | Abbreviated topic |
| `[DATE]` | Current date |

-----

### Step 7: Update BOOTSTRAP-QUERIES.md

Edit `BOOTSTRAP-QUERIES.md` to replace `[REGION-NAME]` and other placeholders with region-specific details.

-----

### Step 8: Create Initial Overview Draft

Create an initial short overview file in `/drafts/overview/` using the region-short-overview template.

File name should be: `[region-name-lowercase-with-hyphens].md`

Example: For "Yellowstone National Park", create `/drafts/overview/yellowstone-national-park.md`

**Initial content to populate:**
- Basic information table
- Geographic coordinates and boundaries
- Brief description (2-3 paragraphs)
- Links to sections to be developed

-----

### Step 9: Set Up Commentary Structure (Optional)

Ask the user: "Would you like to set up a commentary show structure now (for documentaries, podcasts, etc.)?"

If yes, ask for:
- Show name
- Show type (documentary series, podcast, educational content, etc.)

Then create:

```bash
mkdir -p commentaries/[show-name-kebab-case]
mkdir -p commentaries/[show-name-kebab-case]/research
mkdir -p commentaries/[show-name-kebab-case]/seasons
```

And create `commentaries/[show-name]/show-config.md` with show details.

-----

### Step 10: Display Completion Summary

Show the user a summary of the created structure and provide next steps:

```
Project setup complete for [Region Name]!

📁 Directory Structure Verified:
[Show ASCII tree of directories]

📄 Files Updated:
- README.md (replace remaining placeholders as needed)
- BOOTSTRAP-QUERIES.md (customize for your region)
- /drafts/overview/[region-name].md (initial draft created)

✅ Next Steps:

1. Complete the short overview in:
   `/drafts/overview/[region-name].md`

2. Add source materials to `/library/`:
   - Geological surveys → `/library/geological-surveys/`
   - Maps → `/library/maps/`
   - Academic papers → `/library/academic/`
   - Historical documents → `/library/historical-documents/`

3. Begin section documentation (recommended order):
   a. Geography and basic overview
   b. Geology (if primary focus)
   c. Evolutionary history
   d. Natural history (flora and fauna)
   e. Human history
   f. Cultural organization
   g. Significant figures (4-8 biographies)

4. Apply narrative weighting throughout:
   - Flag [UNEXPECTED] content
   - Flag [UNUSUAL] content
   - Flag [TURNING] points
   - Flag [HUMAN] interest stories
   - Flag [PARADOX] resolutions

5. As content is vetted:
   - Move documents from `/drafts/` to `/docs/`
   - Update cross-references
   - Maintain source attribution

6. For commentary creation:
   - Review `/commentaries/templates/`
   - Plan episodes based on `/docs/` content
   - Use narrative highlights as episode anchors

📖 Reference Documents:
- See project-schema.md for detailed organizational guidelines
- See narrative-research-methodology.md for content weighting
- See templates/ for document formatting
- See queries/ for research frameworks

🎯 Primary Deep Dive: [PRIMARY-TOPIC]
Focus special attention on [PRIMARY-TOPIC] documentation.

Happy documenting!
```

-----

## Error Handling

If the user provides incomplete information:
- Ask for clarification
- Offer to proceed with a generic setup that can be customized later
- Suggest reasonable defaults

If directories already exist:
- Alert the user
- Ask whether to:
  - Skip existing directories
  - Merge with existing structure
  - Cancel setup to avoid conflicts

-----

## Customization Options

After completing basic setup, offer these customizations:

1. "Would you like me to create a specific number of biography placeholders?"
   - Create empty biography files for planned significant figures

2. "Would you like to set up multiple commentary shows?"
   - Repeat commentary setup for additional shows

3. "Would you like me to pre-populate any sections based on initial research?"
   - Can begin drafting content immediately

-----

## Maintenance Prompts

Suggest these follow-up commands the user can give:

- "Add a new species document for [Species Name]" → Create draft in natural-history
- "Add a biography for [Figure Name]" → Create draft biography
- "Add a landmark document for [Landmark Name]" → Create draft landmark doc
- "Promote [document] to docs" → Move from drafts to docs with status update
- "Show project status" → Display statistics and current state
- "List all narrative flags" → Show all flagged compelling content

-----

## Narrative Research Reminder

Include this reminder in setup completion:

```
📝 Narrative Research Methodology

Remember to apply narrative weighting throughout all content:

| Flag | Look For |
|------|----------|
| [UNEXPECTED] | Facts that contradict assumptions |
| [PARADOX] | Explanations for apparent contradictions |
| [UNUSUAL] | Statistical rarities and anomalies |
| [HUMAN] | Personal stories and character details |
| [TURNING] | Moments where outcomes hung in balance |

See queries/narrative-research-methodology.md for complete guidance.

Goal: Create content that makes readers say "I never knew that!"
while maintaining rigorous factual accuracy.
```

-----

## Version

- **Version**: 1.0
- **Date**: 2025-11-29
- **Compatible with**: project-schema.md v1.0

-----

*This prompt document is designed to be read and executed by cursor.ai. Update as needed when the schema evolves.*
