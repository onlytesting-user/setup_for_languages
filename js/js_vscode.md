# VS Code Configs

```markdown
{
  // My Personal Configs
  "editor.tabSize": 2,
  "editor.insertSpaces": true,
  "files.autoSave": "afterDelay",
  "editor.formatOnSave": true,
  "files.insertFinalNewline": true,
  "files.trimTrailingWhitespace": true,
  "files.eol": "\n",

  // Configs by Diego (Rocket)
  "editor.fontFamily": "JetBrains Mono",
  "editor.fontLigatures": true,
  "editor.fontSize": 15,
  "editor.lineHeight": 1.5,
  "editor.rulers": [80],
  "editor.semanticHighlighting.enabled": true,
  "editor.minimap.enabled": false,
  "editor.accessibilitySupport": "off",
  "editor.suggestSelection": "first",
  "editor.acceptSuggestionOnCommitCharacter": false,
  "workbench.startupEditor": "newUntitledFile",
  "workbench.editor.labelFormat": "short",
  "workbench.layoutControl.enabled": false,
  "breadcrumbs.enabled": false,
  "window.commandCenter": false,
  "security.workspace.trust.untrustedFiles": "newWindow",
  "git.openRepositoryInParentFolders": "always",
  "update.mode": "default",
  "update.showReleaseNotes": false,
  "terminal.integrated.fontSize": 15,
  "terminal.integrated.fontFamily": "JetBrainsMono Nerd Font",
  "terminal.integrated.defaultProfile.windows": "PowerShell",
  "terminal.integrated.gpuAcceleration": "on",
  "explorer.confirmDragAndDrop": false,
  "explorer.sortOrder": "foldersNestsFiles",
  "explorer.compactFolders": false,
  "explorer.fileNesting.enabled": true,
  "explorer.fileNesting.patterns": {
    "*.ts": "${capture}.js",
    "*.js": "${capture}.js.map, ${capture}.min.js, ${capture}.d.ts",
    "*.jsx": "${capture}.js",
    "*.tsx": "${capture}.ts",
    "*.yaml": "*.yml",
    "tailwind.config.*": "tailwind.config*, postcss.config*",
    "tsconfig.json": "tsconfig*",
    "package.json": ".eslint*, .prettier*, package-lock*, pnpm-*, bun.lockb, vite*",
    "Dockerfile": "Dockerfile*, .docker*",
    "docker-compose.yaml": "docker-compose*",
    ".editorconfig": ".editorconfig*",
    "README.md": "README*, CHANGELOG.md",
    "Makefile": "Makefile*",
    ".gitignore": ".gitignore*, .gitattributes, .gitmodules",
    ".env": ".env*, .envrc"
  },
  "files.associations": {
    "*.js": "javascript",
    "*.jsx": "javascriptreact",
    "*.ts": "typescript",
    "*.tsx": "typescriptreact",
    ".prettierrc": "json",
    "*.html": "html",
    "*.css": "css",
    "*.md": "markdown",
    "*.json": "jsonc",
    "*.prisma": "prisma"
  },

  // Configs for Theme
  "workbench.colorTheme": "Flate Arc Italic",

  // Configs for Prettier
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "prettier.printWidth": 80,
  "prettier.tabWidth": 2,
  "prettier.useTabs": false,
  "prettier.endOfLine": "lf",
  "prettier.proseWrap": "always",
  "prettier.trailingComma": "es5",
  "prettier.semi": true,
  "prettier.singleQuote": true,
  "prettier.arrowParens": "always",
  "prettier.bracketSpacing": true,

  // Configs for ESLint
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": "explicit"
  },
  "eslint.validate": [
    "javascript",
    "javascriptreact",
    "typescript",
    "typescriptreact",
    "graphql"
  ],

  // Configs for JavaScript
  "javascript.suggest.autoImports": true,
  "javascript.updateImportsOnFileMove.enabled": "always",
  "emmet.includeLanguages": {
    "javascript": "javascriptreact"
  }, // @todo-warn Retirar se decidir não usar React
  "emmet.syntaxProfiles": {
    "javascript": "jsx"
  }, // @todo-warn Retirar se decidir não usar React
  "[javascript]": {
    "editor.formatOnSave": true,
    "editor.snippetSuggestions": "top",
    "editor.codeActionsOnSave": {
      "source.organizeImports": "explicit",
      "source.fixAll.ts": "explicit"
    },
    "editor.tabCompletion": "on",
    "editor.quickSuggestions": {
      "other": "on",
      "comments": "off",
      "strings": "on"
    }
  },

  // Configs for TypeScript
  "typescript.tsserver.log": "off",
  "typescript.suggest.autoImports": true,
  "typescript.updateImportsOnFileMove.enabled": "always",
  "typescript.preferences.preferTypeOnlyAutoImports": true,
  "explorer.confirmDelete": false,
  "[typescript]": {
    "editor.formatOnSave": true,
    "editor.snippetSuggestions": "top",
    "editor.codeActionsOnSave": {
      "source.organizeImports": "explicit",
      "source.fixAll.ts": "explicit"
    },
    "editor.quickSuggestions": {
      "other": "on",
      "comments": "off",
      "strings": "on"
    }
  },

  // Configs for Prisma
  "[prisma]": {
    "editor.formatOnSave": true
  },

  // Configs for Code Runner
  "code-runner.runInTerminal": true,
  "code-runner.enableAppInsights": false,

  // Configs for Inline Bookmarks
  "inline-bookmarks.expert.custom.styles": {
    "red": {
      // An item that requires a bugfix
      "gutterIconColor": "#F44336",
      "light": {
        "fontWeight": "bold"
      },
      "dark": {
        "color": "Chocolate"
      }
    },
    "blue": {
      // An item that is awaiting completion
      "gutterIconColor": "#157EFB",
      "light": {
        "fontWeight": "bold"
      },
      "dark": {
        "color": "Chocolate"
      }
    },
    "green": {
      // An item that requires additional review
      "gutterIconColor": "#2FCE7C",
      "light": {
        "fontWeight": "bold"
      },
      "dark": {
        "color": "Chocolate"
      }
    },
    "purple": {
      // Used for generated default snippets
      "gutterIconColor": "#C679E0",
      "light": {
        "fontWeight": "bold"
      },
      "dark": {
        "color": "Chocolate"
      }
    },
    "yellow": {
      // An important note for a specific code section
      "gutterIconColor": "#F4F400",
      "light": {
        "fontWeight": "bold"
      },
      "dark": {
        "color": "Chocolate"
      }
    }
  },
  "inline-bookmarks.expert.custom.words.mapping": {
    "blue": ["@todo[ \\t\\n]"],
    "purple": ["@stub[ \t\\n]"],
    "green": ["@review[ \\t\\n]"],
    "red": ["@fixme[ \\t\\n]"],
    "yellow": ["@note[ \\t\\n]"]
  },

  // Configs for Code Spell Checker
  "cSpell.language": "en,pt,pt_BR",
  "cSpell.userWords": [
    "Ashutosh's",
    "envrc",
    "esbenp",
    "Flate",
    "gitmodules",
    "lockb",
    "Parens",
    "rgba"
  ]
}
```
