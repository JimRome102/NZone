# Kindercare Research Agent Specification

## Agent Purpose

Autonomous agent to research and collect Kindercare location contact information for partnership outreach.

## Agent Tasks

### Phase 1: Location Discovery
- [ ] Search for Kindercare locations using web search
- [ ] Compile list of cities/regions with Kindercare centers
- [ ] Gather addresses and phone numbers
- [ ] Identify if locations are franchise or corporate-owned

### Phase 2: Contact Information Collection
- [ ] Research Center Director names for each location
- [ ] Find director email addresses
- [ ] Find director phone numbers (if available)
- [ ] Identify Area Supervisors (if applicable)
- [ ] Search LinkedIn for additional contact info

### Phase 3: Data Organization
- [ ] Populate `kindercare_contacts.csv` with findings
- [ ] Include all fields: Location name, address, city, state, phone, director name, email, phone, supervisor, LinkedIn URL
- [ ] Add contact status and notes
- [ ] Validate data quality

### Phase 4: Documentation
- [ ] Create summary of research findings
- [ ] Note sources used for data collection
- [ ] Document any challenges or limitations
- [ ] Suggest next steps for outreach

## Data Sources

- Google Maps/Business listings
- Kindercare corporate website and location finder
- LinkedIn (for director profiles)
- Phone directory services
- Business aggregators (ZoomInfo, Apollo.io, Hunter.io if available)

## Output Format

**Primary Output:** `kindercare_contacts.csv`

**Secondary Output:** `docs/research_summary.md` with:
- Total locations found
- Data completeness percentage
- Sources used
- Challenges encountered
- Recommendations for outreach

## Quality Standards

- Email addresses validated (realistic format)
- Phone numbers formatted consistently
- Director names verified where possible
- No duplicate entries
- Complete address information

## Success Criteria

- Minimum 50 Kindercare locations identified
- 80%+ have director contact information
- 60%+ have email addresses
- All data properly formatted in CSV

## Notes

- Focus on major metropolitan areas for initial research
- Prioritize corporate/multiple-location operators
- Document any unverifiable information
- Flag incomplete records for manual follow-up
