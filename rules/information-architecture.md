# Rule: Information Architecture

**Priority:** HIGH
**Category:** Information Architecture

## Description

Information architecture determines how content is structured, labeled, and navigated. If users can't find it, it doesn't exist.

## Navigation Structure

### Core Principles
- Limit primary navigation to 5-7 items
- Use clear, descriptive labels (nouns for sections, verbs for actions)
- Group by user mental models, not org charts
- Provide breadcrumbs for hierarchies deeper than 2 levels
- Users should always know: where am I, where can I go, how do I get back
- Breadth over depth: 7 top-level items beats 3 levels of nesting
- Consistent navigation placement across all pages (spatial memory)
- "Where am I?" should be answerable in 1 second on any screen

### Mobile Considerations
- Use bottom navigation for 3-5 primary actions (most reachable)
- Reserve hamburger menus for secondary navigation only
- Highlight the current section in the navigation bar
- Ensure navigation doesn't consume more than 20% of the viewport

## Content Organization

### Organizational Principles
- **User-centric grouping:** Organize by user goals, not business departments
- **Progressive disclosure:** Show only what's needed; reveal details on demand
- **Consistency:** Same type of content in the same location across pages
- **Scannability:** Clear headings, short paragraphs, visual breaks

### Content Hierarchy
1. **Page title:** What is this page about? (one per page)
2. **Section headings:** Major content groups
3. **Supporting content:** Details within each section
4. **Related content:** Cross-links and supplementary information
6. **F-pattern for text-heavy pages:** key info in the first two words of each line
7. **Z-pattern for visual pages:** eye follows top-left to top-right to bottom-left
  to bottom-right
8. **Above the fold:** 50% of viewing time happens above the fold

### Information Scent
- Labels should clearly indicate what users will find
- Every link and button must clearly signal what's behind it
- Preview content where possible (descriptions, thumbnails, counts)
- Use "trigger words" that match user vocabulary
- Provide visual cues for content types (icons for video, PDF, external links)

### Search as Navigation
- Include search for products with more than 50 content items
- Provide autocomplete suggestions based on popular queries
- Show recent searches for returning users

### Design the Flow, Not Just the Screen
- **Happy path:** the ideal journey from start to finish
- **Edge cases:** 0 items? 1,000 items? Long names? Missing data?
- **Error recovery:** every error needs a clear path back to success
- **Empty states:** the first thing new users see -- make it useful, not "no data"
- **Loading states:** skeleton screens (show structure) beat spinners (show nothing)

## Common Mistakes
- Organizing navigation by internal team structure instead of user needs
- Using jargon or branded terminology users don't understand
- Hiding essential navigation behind a hamburger menu on desktop
- Deep nesting requiring more than 3 clicks to reach important content
- Mirroring the database structure in the UI


## Onboarding Patterns

### Progressive Onboarding (Best for SaaS)
Don't front-load setup. Let users explore, introduce features in context.
- Stripe: one field at a time, value visible immediately
- Notion: empty workspace with contextual "Try this" prompts
- Linear: minimal setup, power features revealed through use

### Guided Onboarding (Best for Complex Products)
Step-by-step wizard when setup is genuinely required.
- "Step 2 of 4" — always show progress
- One action per step, never a wall of fields
- Let users skip non-essential steps
- Celebrate completion with a clear "what's next"

### Value-First Onboarding (Best for Consumer)
Show value before asking for anything.
- Duolingo: first lesson before signup
- Spotify: music plays before account creation
- Canva: template visible before login required

### Key Onboarding Rules
- Time-to-value should be under 60 seconds
- Ask only for what you need RIGHT NOW
- Use possessive language from step one ("Your workspace")
- Every step should feel like progress, not paperwork
- The first action should produce a visible result

## Authentication Patterns

### Login
- Email + password is the baseline
- Social login reduces friction (Google, Apple most trusted)
- Magic link eliminates passwords entirely
- Biometric (Face ID, fingerprint) for mobile apps
- "Remember me" should be on by default

### Signup
- Minimize fields: name + email + password minimum
- Show password requirements BEFORE the user types
- Real-time validation, not post-submission error walls
- Clear value proposition visible during signup
- "Already have an account?" always visible

### Password Reset
- Never say "that email doesn't exist" (security risk)
- "If an account exists, we've sent a reset link"
- Link expires in 1 hour, one-time use
- After reset: auto-login, don't make them sign in again

## E-Commerce Patterns

### Product Pages
- Hero image left, details right (desktop) / image top (mobile)
- Price always visible without scrolling
- Add-to-cart button is the primary CTA, always visible
- Social proof (reviews, ratings) near the CTA
- "In stock" / shipping estimate before the user asks

### Cart
- Persistent cart accessible from every page
- Edit quantity inline (don't force a new page)
- Show running total including estimated shipping
- "Save for later" prevents deletion anxiety
- Related products at bottom, not interrupting the flow

### Checkout
- Guest checkout always available
- Progress indicator: Cart → Shipping → Payment → Confirm
- Auto-fill wherever possible (addresses, saved cards)
- Show order summary at every step
- Security badges near payment fields
- Final review step before charge

## Dashboard Patterns

### Information Dashboard (Monitoring)
- Most critical metric largest and top-left
- Sparklines for trends, not just current numbers
- Color coding: green/yellow/red for status at a glance
- Time range selector globally applied
- Refresh indicator so users know data is current

### Operational Dashboard (Action-Taking)
- Tasks requiring action surfaced prominently
- Filters for status, priority, assignee
- Bulk actions for power users
- Empty state shows success: "All caught up"

### Key Dashboard Rules
- Answer "is everything okay?" in 3 seconds
- Most dashboards show too much — ruthlessly prioritize
- Real-time data needs visible refresh timestamps
- Mobile dashboards show the top 3 metrics, not everything

## Settings Patterns

### Organization
- Group by topic, not alphabetically
- Most-changed settings at the top
- Search within settings for products with many options
- Progressive disclosure: basic visible, advanced collapsed

### Common Mistakes
- Making users save individual fields (auto-save or save all)
- Hiding critical settings in sub-sub-menus
- No confirmation for destructive setting changes
- Settings that require restart without warning
- Toggle labels that don't make it clear what ON means

## Search Patterns

### Search Input
- Tell users what's searchable: "Search projects, files, or members"
- Autocomplete with recent and popular suggestions
- Show results as user types (debounced 200-300ms)
- Search icon OR "⌘K" shortcut for power users

### Results
- Show result count: "12 results for 'budget'"
- Highlight matching terms in results
- Filter/sort options visible but not overwhelming
- No results: suggest corrections, show popular items

## Navigation Patterns

### Top Navigation
Best for: 5-7 main sections, marketing sites, on desktop and simple apps
- Logo left, primary nav center or left, actions right
- Active state clearly marked
- Mobile: hamburger menu (reluctantly — it hides navigation)

### Side Navigation
Best for: 8+ sections, complex apps, frequent switching
- Fixed sidebar with collapsible option
- Group items with clear section headers
- Active state with background highlight
- Collapse to icons for more workspace

### Tab Navigation
Best for: 2-5 views of the same data, mobile apps
- Bottom tabs on mobile (thumb zone)
- Maximum 5 tabs — more requires a "More" overflow
- Active tab always visible without scrolling
- Badge counts for items needing attention

### Bottom Navigation
- Best for mobile apps with 3-5 primary actions
- **Hamburger menu:** Use sparingly; hides navigation and reduces discoverability
- **Tabs:** Best for switching between related views at the same level
---

## Cross-Industry Inspiration

The best solutions come from adjacent industries:

| Your Problem | Look At |
|---|---|
| Complex onboarding | Gaming tutorials (progressive difficulty) |
| Trust in transactions | Banking (security reassurance patterns) |
| Content discovery | Streaming services (recommendation UX) |
| Collaboration | Multiplayer games (real-time presence) |
| Data input | Tax software (wizard patterns, auto-fill) |
| Retention | Fitness apps (streaks, progress, milestones) |
| Emergency actions | Aviation cockpits (error prevention, confirmation) |

Don't copy screens — extract the principle and apply it to your context.
