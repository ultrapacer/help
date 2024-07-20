# help

### adding new files

1. save the file in .md format in the _/docs_ folder
2. add the file into the _sidebar.json_ file

```
  ...
    },
    {
      "route": {
        "name": "dashboard",
        "params": {
          "view": "runs"
        },
        "query": {
          "time": "past"
        }
      },
      "file": "dashboard-pastruns"
    },
  ...
```

3. the docs will appear in the same order that they are in the .json file
