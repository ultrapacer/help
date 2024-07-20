# help

### here is how it works:

the sidebar help pulls live from this repository
the sidebar.json file include an array of documents with filter criteria in the "route" object
the help documenation utilizes the URL **name** and **query** to know which content to render, as shown:\n
https://ultrapacer.com/name/blah/blah?query1=val1&query2=val2
note that the names

So, given the url https://ultrapacer.com/dashboard/?view=runs&time=past:\n
_dashboard_ is the route name
_runs_ is a query
_time_ is a query

the sidebar will show all matching items in order.

### adding new files

1. save the file in .md format in the _/docs_ folder
2. add the file into the _sidebar.json_ file

```
  ...
    },
    {
      "page": "dashboard",
      "query": {
        "time": "past",
        "view": "runs"
      },
      "file": "dashboard-pastruns.md"
    },
  ...
```

3. the docs will appear in the same order that they are in the .json file
