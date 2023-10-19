---
cssclass: academia, academia-rounded, wideTable
---
# <mark>Spaced Repetition By Topics</mark>
```button
name Fold
type command
action Fold all headings and lists
```
^button-Fold
## Core Systems Review Cards
```dataview
TABLE sr-due AS "DUE", sr-ease AS "Ease"
FROM #review/card/cardiology or #review/card/GI or #review/card/renal or #review/card/pulm or #review/card/neuro
WHERE sr-due >= date(today) - dur(1000 day) and sr-due <= date(today) + dur(0 day)
SORT sr-due ASC
LIMIT 10
```

## <mark class="hltr-red">Cardiology</mark> 
### Reviews
```dataview
TABLE sr-due AS "DUE", sr-ease AS "Ease"
FROM #review/card/cardiology or #review/topicnote/cardiology 
WHERE sr-due >= date(today) - dur(1000 day)
SORT sr-due ASC
LIMIT 5
```

### New
```dataview
TABLE sr-due AS "DUE", sr-ease AS "Ease"
FROM #review/card/cardiology or #review/topicnote/cardiology 
SORT sr-due ASC
LIMIT 5
```
## <mark class="hltr-orange">Renal</mark> 
### Reviews
```dataview
TABLE sr-due AS "DUE", sr-ease AS "Ease"
FROM #review/card/nephro or #review/topicnote/nephro or #review/card/renal or #review/topicnote/nephro
WHERE sr-due >= date(today) - dur(1000 day)
SORT sr-due ASC
LIMIT 5
```
### New
```dataview
TABLE sr-due AS "DUE", sr-ease AS "Ease"
FROM #review/card/nephro or #review/topicnote/nephro or #review/card/renal or #review/topicnote/nephro
SORT sr-due ASC
LIMIT 5
```
## <mark class="hltr-yellow">ID</mark> 
### Reviews
```dataview
TABLE sr-due AS "DUE", sr-ease AS "Ease"
FROM #review/card/ID or #review/topicnote/id 
WHERE sr-due >= date(today) - dur(1000 day)
SORT sr-due ASC
LIMIT 5
```
### New
```dataview
TABLE sr-due AS "DUE", sr-ease AS "Ease"
FROM #review/card/ID or #review/topicnote/id 
SORT sr-due ASC
LIMIT 5
```
## <mark class="hltr-blue">Pulmonology</mark> 
### Reviews
```dataview
TABLE sr-due AS "DUE", sr-ease AS "Ease"
FROM #review/card/pulm or #review/topicnote/pulm 
WHERE sr-due >= date(today) - dur(1000 day)
SORT sr-due ASC
LIMIT 5
```
### New
```dataview
TABLE sr-due AS "DUE", sr-ease AS "Ease"
FROM #review/card/pulm or #review/topicnote/pulm 
SORT sr-due ASC
LIMIT 5
```
## <mark class="hltr-purple">Neuro</mark> 
### Reviews
```dataview
TABLE sr-due AS "DUE", sr-ease AS "Ease"
FROM #review/card/neuro or #review/topicnote/neuro 
WHERE sr-due >= date(today) - dur(1000 day)
SORT sr-due ASC
LIMIT 5
```
### New
```dataview
TABLE sr-due AS "DUE", sr-ease AS "Ease"
FROM #review/card/neuro or #review/topicnote/neuro 
SORT sr-due ASC
LIMIT 5
```

---
## <mark class="hltr-grey">GI</mark> 
### Reviews
```dataview
TABLE sr-due AS "DUE", sr-ease AS "Ease"
FROM #review/card/GI or #review/topicnote/GI 
WHERE sr-due >= date(today) - dur(1000 day)
SORT sr-due ASC
LIMIT 5
```
### New
```dataview
TABLE sr-due AS "DUE", sr-ease AS "Ease"
FROM #review/card/GI or #review/topicnote/GI 
SORT sr-due ASC
LIMIT 5
```
# <mark>Spaced Repetition By Time</mark>
## Today
```dataview
LIST
FROM #review/topicnote
SORT sr-due ASC
WHERE sr-due >= date(today) - dur(2 day) and sr-due <= date(today) + dur(2 day)
LIMIT 5
```
- ---
```dataview
LIST
FROM #review/card 
SORT sr-due ASC
WHERE sr-due >= date(today) - dur(2 day) and sr-due <= date(today) + dur(1 day)
LIMIT 20
```

## Most Challenging & Overdue Reviews
```dataview
TABLE sr-due AS "DUE", sr-ease AS "Ease"
FROM #review/card 
SORT sr-due ASC
WHERE sr-due >= date(today) - dur(1000 day) and sr-due <= date(today) + dur(1 day)
WHERE sr-ease <= (200)
LIMIT 5
```

---
## Recently Edited Review Cards

```dataview 
TABLE file.mtime as Modified, sr-due AS "DUE", sr-ease AS "Ease"
FROM #review/card  
WHERE date(now) - file.mtime <= dur(3 days) 
SORT file.mtime desc 
Limit 10
```
## Recently Created Topic Notes

```dataview 
TABLE file.ctime as Created, sr-due AS "DUE", sr-ease AS "Ease"
FROM #review/topicnote 
WHERE date(now) - file.ctime <= dur(14 days) 
SORT file.ctime desc 
```

# <mark>Spaced Repetition By Type</mark>
## ==Topic Notes==
```dataview
CALENDAR sr-due AS "DUE"
FROM "01. Topic Notes"
SORT sr-due ASC
WHERE sr-due >= date(today) - dur(60 day)
```
## ==Quizzes & Flashcards==
```dataview 
LIST
FROM #review/quiz or #flashcards
WHERE sr-due <= date(today) or ""
SORT sr-due DESC
LIMIT 10
```

## Overdue Cards
- **More than a month overdue**
	```dataview
	TABLE sr-due AS "DUE", sr-ease AS "Ease"
	FROM #review/card 
	SORT sr-due ASC
	WHERE sr-due >= date(today) - dur(1000 day) and sr-due <= date(today) - dur(30 day)
	LIMIT 5
	```
- **More than three months overdue**
	```dataview
	Table sr-due AS "DUE", sr-ease AS "Ease"
	FROM #review/card 
	SORT sr-due ASC
	WHERE sr-due >= date(today) - dur(1000 day) and sr-due <= date(today) - dur(90 day)
	LIMIT 5
	```

## Suspended Cards

```dataview 
LIST
FROM #review/suspend or "/Users/danielbergholz/Documents/Second Brain/01. Topic Notes/Topic Notes - Buried"
SORT file.mtime desc 
```











## Spaced Repetition Decks in Progress
## Unresolved Questions
```dataview
LIST
FROM #unresolved 
```
## Quiz Questions
```dataview 
TASK FROM #review 
WHERE !completed
```