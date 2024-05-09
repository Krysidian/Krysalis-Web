# Category Database
---

## Character Notes


```dataview
TABLE WITHOUT ID file.link AS Note, character AS Character, focus AS Focus, TAGS AS Tags
WHERE contains(category, "character") OR contains(category, "Character") AND !contains(tags, "template")
SORT file.mtime DESC
```

---

## Location Notes

```dataview
TABLE WITHOUT ID file.link AS Note, character AS Character, focus AS Focus, TAGS AS Tags
WHERE contains(category, "location") OR contains(category, "Location") AND !contains(tags, "template")
SORT file.mtime DESC
```
---
## Principle Notes

```dataview
TABLE WITHOUT ID file.link AS Note, character AS Character, focus AS Focus, TAGS AS Tags
WHERE contains(category, "principle") OR contains(category, "Principle") AND !contains(tags, "template")
SORT file.mtime DESC
```
---
## Vibe Notes

```dataview
TABLE WITHOUT ID file.link AS Note, character AS Character, focus AS Focus, TAGS AS Tags
WHERE contains(category, "vibe") OR contains(category, "Vibe") AND !contains(tags, "template")
SORT file.mtime DESC
```
---
## Quote Notes

```dataview
TABLE WITHOUT ID file.link AS Note, character AS Character, focus AS Focus, TAGS AS Tags
WHERE contains(category, "quote") OR contains(category, "Quote") AND !contains(tags, "template")
SORT file.mtime DESC
```
---
## Unsorted

```dataview
TABLE WITHOUT ID file.link AS Note, character AS Character, focus AS Focus, TAGS AS Tags
FROM "StoryNotes"
WHERE category = null
SORT file.mtime DESC
```
---