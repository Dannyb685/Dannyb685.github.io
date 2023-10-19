# Recent Files

```dataview 
TABLE file.ctime as Created FROM "" WHERE date(now) - file.ctime <= dur(3 days) SORT file.ctime desc 
```
