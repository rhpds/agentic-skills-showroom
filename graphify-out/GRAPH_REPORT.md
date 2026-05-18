# Graph Report - .  (2026-05-18)

## Corpus Check
- Corpus is ~25,201 words - fits in a single context window. You may not need a graph.

## Summary
- 102 nodes · 119 edges · 19 communities (15 shown, 4 thin omitted)
- Extraction: 95% EXTRACTED · 5% INFERRED · 0% AMBIGUOUS · INFERRED: 6 edges (avg confidence: 0.9)
- Token cost: 101,948 input · 0 output

## Community Hubs (Navigation)
- [[_COMMUNITY_Course Curriculum Design|Course Curriculum Design]]
- [[_COMMUNITY_Dolt Repo State|Dolt Repo State]]
- [[_COMMUNITY_Project Tooling Config|Project Tooling Config]]
- [[_COMMUNITY_Antora Build Pipeline|Antora Build Pipeline]]
- [[_COMMUNITY_Showroom UI Links|Showroom UI Links]]
- [[_COMMUNITY_Dev Mode Attributes|Dev Mode Attributes]]
- [[_COMMUNITY_Beads Metadata|Beads Metadata]]
- [[_COMMUNITY_Export State Tracking|Export State Tracking]]
- [[_COMMUNITY_Claude Code Hooks|Claude Code Hooks]]
- [[_COMMUNITY_Dolt Backup Remote|Dolt Backup Remote]]
- [[_COMMUNITY_Dolt Origin Remote|Dolt Origin Remote]]
- [[_COMMUNITY_Backup State|Backup State]]
- [[_COMMUNITY_Local Permissions|Local Permissions]]
- [[_COMMUNITY_Dolt Server Config|Dolt Server Config]]
- [[_COMMUNITY_Beads Documentation|Beads Documentation]]

## God Nodes (most connected - your core abstractions)
1. `Skills Course Implementation Plan` - 12 edges
2. `Antora Site Playbook (site.yml)` - 7 edges
3. `remotes` - 6 edges
4. `backups` - 6 edges
5. `branches` - 6 edges
6. `Claude Code Agent Skills` - 6 edges
7. `head` - 5 edges
8. `origin` - 5 edges
9. `backup_export` - 5 edges
10. `GitHub Pages CI/CD Workflow` - 5 edges

## Surprising Connections (you probably didn't know these)
- `Cursor .cursorrules` --semantically_similar_to--> `Claude Code Agent Skills`  [INFERRED] [semantically similar]
  docs/superpowers/specs/2026-05-05-skills-course-design.md → CLAUDE.md
- `Perles TUI Configuration` --references--> `Beads Issue Tracker`  [INFERRED]
  .perles/config.yaml → AGENTS.md
- `Skills Course Implementation Plan` --references--> `AsciiDoc Showroom Conventions`  [EXTRACTED]
  docs/superpowers/plans/2026-05-05-skills-course.md → CLAUDE.md
- `Skills Course Implementation Plan` --references--> `Antora Site Playbook (site.yml)`  [EXTRACTED]
  docs/superpowers/plans/2026-05-05-skills-course.md → site.yml
- `Skills Course Implementation Plan` --references--> `Showroom UI Configuration (ui-config.yml)`  [EXTRACTED]
  docs/superpowers/plans/2026-05-05-skills-course.md → ui-config.yml

## Hyperedges (group relationships)
- **Conference Toolkit Skills Bundle** — showroom_skills_course_conference_toolkit, showroom_skills_course_abstract_writer, showroom_skills_course_conf_finder, showroom_skills_course_trip_report [EXTRACTED 1.00]
- **Three-Layer Skill Composition (Harness/Domain/Workflow)** — showroom_skills_course_superpowers, showroom_skills_course_conference_toolkit, showroom_skills_course_beads, showroom_skills_course_layered_ecosystem [EXTRACTED 1.00]
- **Antora Site Build Pipeline** — showroom_skills_course_site, content_antora, showroom_skills_course_rhdp_ui_bundle, workflows_gh_pages, showroom_skills_course_github_pages [EXTRACTED 1.00]

## Communities (19 total, 4 thin omitted)

### Community 0 - "Course Curriculum Design"
Cohesion: 0.21
Nodes (17): Skills Course Implementation Plan, abstract-writer Skill, Claude Code Agent Skills, conf-finder Skill, conference-toolkit Marketplace, Cursor .cursorrules, Deep Agents (Programmatic Skills), Layered Skill Ecosystem (+9 more)

### Community 1 - "Dolt Repo State"
Cohesion: 0.35
Nodes (7): backups, branches, main, head, head, remote, remotes

### Community 2 - "Project Tooling Config"
Cohesion: 0.22
Nodes (9): Beads Configuration File, Dolt SQL Server Configuration, Agent Instructions (AGENTS.md), AsciiDoc Showroom Conventions, Beads Issue Tracker, Project Instructions (CLAUDE.md), Dolt Database Backend, Perles TUI Configuration (+1 more)

### Community 3 - "Antora Build Pipeline"
Cohesion: 0.31
Nodes (9): Antora Component Descriptor (antora.yml), Antora Static Site Generator, GitHub Pages Deployment, Antora Lunr Search Extension, Antora Mermaid Extension, RHDP Showroom UI Theme Bundle, Antora Site Playbook (site.yml), Antora Tabs Extension (+1 more)

### Community 4 - "Showroom UI Links"
Cohesion: 0.25
Nodes (8): Showroom UI Links Dropdown Screenshot, AnsibleFest Branding, GitHub Sourced Container Module, Links Dropdown Menu, Red Hat Summit 2024 Branding, RPM Native Container Module, Showroom Split-Pane Layout, Sidebar Navigation Panel

### Community 5 - "Dev Mode Attributes"
Cohesion: 0.33
Nodes (7): Dev Mode Attributes Page Screenshot, Antora Component Attributes (master@modules), Showroom Attribute Variables (guid, ssh_user, ssh_password, bastion hostname), dev-mode.js Antora Extension, Showroom UI (Red Hat Summit 2024), Sidebar Navigation (RPM Native Container, GitHub Sourced Container, Dev Mode), site.yml (Antora Playbook)

### Community 6 - "Beads Metadata"
Cohesion: 0.33
Nodes (5): backend, database, dolt_database, dolt_mode, project_id

### Community 7 - "Export State Tracking"
Cohesion: 0.4
Nodes (4): issues, last_dolt_commit, memories, timestamp

### Community 8 - "Claude Code Hooks"
Cohesion: 0.4
Nodes (4): hooks, PostToolUse, PreToolUse, SessionStart

### Community 9 - "Dolt Backup Remote"
Cohesion: 0.4
Nodes (5): fetch_specs, name, params, url, backup_export

### Community 10 - "Dolt Origin Remote"
Cohesion: 0.4
Nodes (5): fetch_specs, name, params, url, origin

## Knowledge Gaps
- **43 isolated node(s):** `SessionStart`, `PostToolUse`, `PreToolUse`, `allow`, `database` (+38 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **4 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `Skills Course Implementation Plan` connect `Course Curriculum Design` to `Project Tooling Config`, `Antora Build Pipeline`?**
  _High betweenness centrality (0.066) - this node is a cross-community bridge._
- **Why does `Antora Site Playbook (site.yml)` connect `Antora Build Pipeline` to `Course Curriculum Design`?**
  _High betweenness centrality (0.037) - this node is a cross-community bridge._
- **Why does `Layered Skill Ecosystem` connect `Course Curriculum Design` to `Project Tooling Config`?**
  _High betweenness centrality (0.034) - this node is a cross-community bridge._
- **What connects `SessionStart`, `PostToolUse`, `PreToolUse` to the rest of the system?**
  _43 weakly-connected nodes found - possible documentation gaps or missing edges._