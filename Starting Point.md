## Button to create New Blog Post

```button
name Create New Post
type command
action QuickAdd: Add Blog Post
color blue
```

## Blog

### Data Science 
608804
```dataview
TABLE summary as "Summary", status as "Status"
FROM "Data Science"
SORT file.name ASCENDING
```


### ML
```dataview
TABLE summary as "Summary"
FROM "ML"
SORT file.name ASCENDING
```


## Productivity
```dataview
TABLE summary as "Summary"
FROM "Productivity"
SORT file.name ASCENDING
```