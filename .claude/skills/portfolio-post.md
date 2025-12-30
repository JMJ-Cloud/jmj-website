# Portfolio Post Creation Skill

This skill helps create new portfolio posts following the established format and guidelines.

## Frontmatter Structure

Every portfolio post must include the following YAML frontmatter:

```yaml
---
title: "Project Title"
status: "Active" | "Completed" | "In Progress"
summary: "One to two sentence overview highlighting the core value and key outcome"
technologies:
  - "Technology 1"
  - "Technology 2"
  - "Technology 3"
industry: "Industry Name"
metrics:
  - "Key metric or achievement 1"
  - "Key metric or achievement 2"
  - "Key metric or achievement 3"
featured: true | false
order: 1  # Lower numbers appear first
---
```

## Required Content Sections

### 1. Project Overview
- High-level description of the project
- Primary objectives and scope
- Client context (anonymized if needed)
- 2-3 paragraphs maximum

### 2. Business Challenge
- Clear problem statement
- Bullet points describing specific pain points
- Quantify impact where possible
- Focus on business/user needs, not technical details

### 3. Solution Architecture

**Start with Core Technologies:**
- List primary technical stack
- Explain why each technology was chosen
- Keep focused on key components

**Then describe Key Functional Modules:**
- Break down solution into major components
- Use ### for module headers
- 2-4 bullet points per module
- Focus on business functionality, not implementation

### 4. Technical Highlights
- Deep technical implementation details
- Use bold headers for categories like:
  - **Framework/Architecture Pattern:**
  - **Data Quality & Validation:**
  - **Performance Optimization:**
  - **Security/Scalability/Integration:**
- Include specific techniques, patterns, tools used
- Bullet points for clarity

### 5. Current Status & Progress (for active projects)
Include subsections:
- **Platform Foundation (Complete):**
- **Active Development Modules:**
- **Early Results:**
- **Next Steps:**

OR for completed projects:

### 5. Results & Impact
- Quantified outcomes
- User feedback
- Performance improvements
- Business value delivered

### 6. Deliverables
- Bullet list of concrete outputs
- Documentation
- Code/applications
- Training materials
- Support handoff

### 7. Why This Matters
- Highlight demonstrated expertise areas
- Use bold for skill categories
- Connect to broader capabilities
- 4-6 key expertise areas
- Format: "**Skill Area** - Specific demonstration"

## Writing Style Guidelines

1. **Professional but accessible** - Avoid jargon where possible
2. **Results-focused** - Emphasize outcomes over activities
3. **Specific and concrete** - Use real examples, not generic statements
4. **Active voice** - "Delivered" not "Was delivered"
5. **Consistent formatting** - Match the pattern shown above
6. **Bullet points** - Use for lists, features, and benefits
7. **Section headers** - Use ## for main sections, ### for subsections

## Metrics Guidelines

Metrics should be:
- **Quantifiable** when possible (e.g., "50% reduction in processing time")
- **Specific** to project achievements
- **Business-focused** (user impact, efficiency, scale)
- **Concise** (one line each)

Examples:
- "Processing 10M+ records daily"
- "Reduced deployment time from hours to minutes"
- "Supporting 500+ concurrent users"
- "99.9% uptime in production"

## File Naming Convention

Use kebab-case for filenames:
- `project-name.md`
- Place in `src/content/projects/`

## Summary Writing Tips

The summary appears in project cards and should:
- Be 1-2 sentences maximum
- Start with action verb: "Delivering", "Built", "Designed"
- Include key technology and business outcome
- Mention client context if relevant
- Avoid buzzwords and marketing speak

## Technology List Guidelines

- List most important technologies first
- Include 3-6 key technologies
- Use official product names
- Be specific (e.g., "Oracle EBS R12.2" not just "Oracle")

## Order Priority

- Lower numbers = higher priority (appear first)
- Featured posts appear before non-featured
- Use order to sequence projects by importance/recency
