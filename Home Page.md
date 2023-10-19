### Topic Reviews
```dataview
LIST
FROM #review/topicnote
SORT sr-due ASC
WHERE sr-due >= date(today) - dur(14 day) and sr-due <= date(today) + dur(1 day)
LIMIT 5
```
### Review Cards
```dataview
LIST
FROM #review/card 
SORT sr-due ASC
WHERE sr-due >= date(today) - dur(7 day) and sr-due <= date(today) + dur(1 day)
LIMIT 10
```
### Recent Topics
```dataview
LIST
FROM #review/topicnote
SORT file.mtime DESC
LIMIT 10
```