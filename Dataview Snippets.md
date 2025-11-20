# Dataview Snippets (copy into any note)

Below are the same Dataview queries shown in the Templates note, isolated for easy copy-paste.

## 1) Unfinished tasks grouped by file

```dataview
task from "Database Roadmap"
where !completed
group by file.link
sort file.name asc
```

## 2) Topic notes with frontmatter fields

```dataview
table status, difficulty, created
from "Database Roadmap"
where contains(file.path, "01 - Fundamentals") or contains(file.path, "02 - RDBMS")
sort status asc
```

## 3) Projects and open tasks

```dataview
table file.link as Project, length(filter(file.tasks, (t) => t.completed = false)) as "Open Tasks"
from "Database Roadmap"
where contains(tags, "project")
```

## 4) Files with most open tasks

```dataview
table file.link, length(filter(file.tasks, (t) => !t.completed)) as "Open Tasks"
from "Database Roadmap"
sort "Open Tasks" desc
limit 20
```

Notes:

- If Dataview returns no results, check plugin is enabled and the path matches your vault layout.
- You can embed these queries directly in `00 - Roadmap Overview.md` to create a dashboard.
