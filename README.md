# termwebsites

welcome to the repository for termwebsites on the termweb! this is the repository [termwebbrowser](https://github.com/sillybreakfast/termwebbrowser/) fetches from to display content.

## termwebsite structure

### directory

when the program is given an input, it goes into this fetching URL:
```
https://raw.githubusercontent.com/sillybreakfast/termwebsites/refs/tags/{latest release name}/sites/{input}/.json
```

please note that `/.json` is appended to the end of the URL. this means an input of `helloworld` would fetch `sites/helloworld/.json`. do not use this format: `helloworld.json`- this will not work. all JSON files should be named `.json`.

### JSON fields

currently, there are only two fields termwebbrowser recognizes:
- `title`: the title of the page (not the same as the name placed in the URL).
- `content`: the content on the page.
