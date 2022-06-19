---
layout: page
show_meta: true
title: "Dataview Queries"
subheadline: "How to use it"
breadcrumb: true
categories:
    - notes
    - obsidian
---

## Showcases

### Relevant Daily Notes for Weekly Review
In this particular query, it is assumed that the weekly note is in the "yyyy-[W]ww" format (e.g. `2022-W05.md`) and the daily notes in "yyyy-mm-dd" format (e.g. `2022-02-01.md`). It will pull the daily notes related to Week 5 of 2022 (31 Jan 2022 - 6 Feb 2022)
~~~
```dataview
TABLE
  dateformat(file.day,"ccc, MMM dd") AS Date
FROM
  "Daily Notes"
WHERE
  file.day.weekyear = number(split(this.file.name, "W")[1]) AND
  contains(file.name, "-W")
SORT
  file.name ASC
```
~~~

### Finding pages with no linking or tags
To get status that a note has no backlinks, outgoing links or tags, we use `length()` function to test if it is `0`. If it is, it means the tested field's properties is empty or null.
~~~
```dataview
TABLE
  rows.file.link as "MD Files"
WHERE
  (length(file.inlinks) =0 AND length(file.outlinks) =0) OR
  (length(file.tags) =0)
GROUP BY
  file.folder
```
~~~
