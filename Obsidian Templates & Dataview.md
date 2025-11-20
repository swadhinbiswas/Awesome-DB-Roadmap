# Obsidian Templates & Dataview Snippets

This note contains ready-to-use templates and Dataview snippets to speed up learning inside this vault.

---

## Quick setup

- Install Obsidian Community Plugins:
  - **Templates** (core plugin may suffice) or **Templater** for advanced placeholders
  - **Dataview** (for powerful queries across notes)
- Place templates in `Templates/` (already created in this vault).
- Optionally set your templates folder in Settings → Templates.

---

## Topic Note Template (use as `Templates/Topic Template.md`)

Use this for every concept note (e.g., `ACID.md`, `Indexes.md`). If you use Templater, replace `{{DATE}}` / `{{TITLE}}` with Templater variables.

```
---
created: {{DATE}}
tags: [topic, database]
status: todo
difficulty: intermediate
---

# {{TITLE}}

## 🎯 Goals
- [ ] Goal 1
- [ ] Goal 2

## 📚 Checklist
- [ ] Learn core concept
- [ ] Run at least one practical example
- [ ] Write a short note summarizing the key trade-offs

## 🧪 Practice
- [ ] Example task 1
- [ ] Example task 2

## 🔗 Related
- [01 - Fundamentals](01%20-%20Fundamentals.md)
- [02 - RDBMS](02%20-%20RDBMS.md)

```

---

## Project Template (use as `Templates/Project Template.md`)

```
---
created: {{DATE}}
tags: [project]
status: plan
difficulty: advanced
---

# {{PROJECT_TITLE}}

## Summary
Short description.

## Objectives
- [ ] Objective 1
- [ ] Objective 2

## Technologies
- PostgreSQL / Redis / Kafka / Dataview etc.

## Steps
1. Design schema / data model
2. Implement basic services
3. Add tests and instrumentation
4. Deploy with Docker Compose

## Artifacts
- Schema file: `schema.sql`
- Docker compose: `docker-compose.yml`

## Retro
- What went well
- What to improve

```

---

## Dataview snippets (examples)

Place these in any note to run them. They assume Dataview plugin is enabled.

1. List unfinished tasks in the `Database Roadmap` folder grouped by file:

```dataview
task from "Database Roadmap"
where !completed
group by file.link
sort file.name asc
```

2. Show all topic notes with a `status` field and their status:

```dataview
table status, difficulty, created
from "Database Roadmap"
where contains(file.path, "01 - Fundamentals") or contains(file.path, "02 - RDBMS")
sort status asc
```

3. Project overview: list notes tagged `project` and show incomplete objectives (tasks):

```dataview
table file.link as Project, length(filter(file.tasks, (t) => t.completed = false)) as "Open Tasks"
from "Database Roadmap"
where contains(tags, "project")
```

4. Show files with most unchecked tasks (helps find unfinished topics):

```dataview
table file.link, length(filter(file.tasks, (t) => !t.completed)) as "Open Tasks"
from "Database Roadmap"
sort "Open Tasks" desc
limit 20
```

---

## Tagging & frontmatter suggestions

- Use `tags` like: `#topic`, `#project`, `#practice`
- Use frontmatter keys: `status: todo/in-progress/done`, `difficulty: beginner/intermediate/advanced`, `created: YYYY-MM-DD`

---

If you want, I can convert a few existing notes to use the Topic Template frontmatter and add Dataview panels to `00 - Roadmap Overview.md` to show your progress automatically.
