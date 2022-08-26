# remarkable-brackets

## This plugin for remarkable allows you to add custom double bracket syntaxes to your remarkable parser.


For example:

```js
var rm_brackets = require("remarkable-brackets");
var Remarkable = require("remarkable");

var remarkable = new Remarkable("full", {html: true, breaks: true})
remarkable.use(rm_brackets({name: "cloze", :opener "{", closer: "}"}));
```

Now you can use syntax like:

```md
This is my {{new syntax}}.
```
