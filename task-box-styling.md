# Task Box Styling

#journaling #bujo #vscode

The `publicus.org-checkbox` extension is nice to render boxes inspired by bullet journaling. But the general theme is not what I like. I settup custom settings using the `fabiospampinato.vscode-highlight` extension resulting in this:

![picture 1](../images/2020-11-18-1605713806172.png)

Sadly, those color are not rendered on github but as journal is supposed to be used throughout the day in VS code, thus, this is not an issue.

Highlight settings:

```json
  "highlight.regexes": {
    "(\\- ?\\[ ?\\].*)": [
        {
        "color": "#ff0f16",
        "fontWeight": "bold"
        }
    ],
    "(\\- ?\\[x\\] ?:? ?)(.*)": [
        {
        "color": "#6bf285",
        "fontWeight": "bold",
        },
        {
        "color": "#6bf285",
        "fontWeight": "bold",
        "textDecoration": "line-through"
        }
    ],
        "(\\- ?\\[\\/\\].*)": [
        {
            "color": "#1d58ff",
            "fontWeight": "bold"
        }
        ],
    "(\\- ?\\[\\>\\].*)": [
        {
        "color": "#ffa200",
        "fontWeight": "bold"
        }
    ],
    "(\\- ?\\[\\<\\].*)": [
        {
        "color": "#3eb563",
        "fontWeight": "bold"
        }
    ],
    "(\\- ?\\[\\-\\] ?:? ?)(.*)": [
        {
        "color": "#8b8b8b",
        "fontWeight": "bold"
        },
        {
        "color": "#8b8b8b",
        "fontWeight": "bold",
        "textDecoration": "line-through",
        }
    ],
    "(\\- ?\\[\\o\\].*)": [
        {
        "color": "#faabf0",
        "fontWeight": "bold"
        }
    ]
}
```