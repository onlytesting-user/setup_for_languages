# Code for omyposh

```
{
    "$schema": "https://raw.githubusercontent.com/JanDeDobbeleer/oh-my-posh/main/themes/schema.json",
    "blocks": [
      {
        "alignment": "left",
        "segments": [
          {
            "foreground": "#ee5959", //#F09456
            "properties": {
              "style": "folder"
            },
            "style": "plain",
            "template": "{{ .Path }}/ ",
            "type": "path"
          },
          {
            "foreground": "#f967bf", //#F797D0
            "properties": {
              "fetch_status": true
            },
            "style": "plain",
            "template": "<#ffffff>on</> {{ .HEAD }}{{if .BranchStatus }} {{ .BranchStatus }}{{ end }}{{ if .Working.Changed }} \uf044 {{ .Working.String }}{{ end }}{{ if and (.Working.Changed) (.Staging.Changed) }} |{{ end }}{{ if .Staging.Changed }} \uf046 {{ .Staging.String }}{{ end }} ",
            "type": "git"
          },
          {
            "foreground": "#7ad971", //#65D25A
            "properties": {
              "fetch_version": true
            },
            "style": "plain",
            "template": "<#ffffff>via</> \ue235 {{ if .Venv }} {{ end }}{{ .Full }} ",
            "type": "python"
          }
        ],
        "type": "prompt"
      },
      {
        "alignment": "right",
        "segments": [
          {
            "foreground": "#ffffff",
            "leading_diamond": "\ue641",
            "properties": {
              "style": "roundrock",
              "threshold": 0
            },
            "style": "diamond",
            "template": " {{ .FormattedMs }} ",
            "type": "executiontime"
          }
        ],
        "type": "prompt"
      },
      {
        "alignment": "left",
        "newline": true,
        "segments": [
          {
            "foreground": "#fff200",
            "style": "plain",
            "template": "\u2b9e ",
            "type": "text"
          }
        ],
        "type": "prompt"
      }
    ],
    "final_space": true,
    "version": 2
  }
```
