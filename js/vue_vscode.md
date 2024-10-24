# VS Code Configs

```markdown
{
  // * Editor Configs
  "editor.fontFamily": "JetBrains Mono",
  "editor.fontLigatures": true,
  "editor.fontSize": 15,
  "editor.lineHeight": 1.5,
  "editor.rulers": [
    80
  ],
  "editor.semanticHighlighting.enabled": true,
  "editor.minimap.enabled": false,
  "editor.accessibilitySupport": "off",
  "editor.suggestSelection": "first",
  "editor.acceptSuggestionOnCommitCharacter": false,
  "editor.stickyScroll.enabled": false,
  "editor.codeLens": true,
  "editor.glyphMargin": true,
  "editor.insertSpaces": true,
  "editor.tabSize": 4,
  "editor.indentSize": "tabSize",
  "editor.snippetSuggestions": "top",
  "editor.tabCompletion": "on",
  "editor.quickSuggestions": {
    "other": "on",
    "comments": "off",
    "strings": "off"
  },

  // * Files Configs
  "files.eol": "\n",
  "files.autoSave": "afterDelay",
  "files.trimTrailingWhitespace": true,
  "files.insertFinalNewline": true,
  "files.associations": {
    "*.js": "javascript",
    "*.ts": "typescript",
    "*.vue": "vue",
    ".prettierrc": "json",
    "*.html": "html",
    "*.css": "css",
    "*.md": "markdown",
    "*.json": "jsonc",
    "*.prisma": "prisma",
    "*.yaml": "yaml",
    ".env": "dotenv"
  },
  "files.exclude": {
    "**/.git": true,
    "**/.svn": true,
    "**/.hg": true,
    "**/CVS": true,
    "**/.DS_Store": true,
    "**/Thumbs.db": true
  },

  // * Workbench Configs
  "workbench.startupEditor": "newUntitledFile",
  "workbench.editor.labelFormat": "short",
  "workbench.layoutControl.enabled": false,
  "workbench.tree.enableStickyScroll": false,
  "workbench.editor.empty.hint": "hidden",

  // * Terminal Configs
  "terminal.integrated.fontSize": 15,
  "terminal.integrated.fontFamily": "JetBrainsMono Nerd Font",
  "terminal.integrated.defaultProfile.windows": "PowerShell",
  "terminal.integrated.gpuAcceleration": "on",
  "terminal.integrated.showExitAlert": false,

  // * Explorer Configs
  "explorer.confirmDelete": false,
  "explorer.confirmDragAndDrop": false,
  "explorer.sortOrder": "foldersNestsFiles",
  "explorer.compactFolders": false,
  "explorer.fileNesting.enabled": true,
  "explorer.fileNesting.patterns": {
    "*.ts": "${capture}.js",
    "*.js": "${capture}.js.map, ${capture}.min.js, ${capture}.d.ts",
    "*.vue": "${capture}.ts, ${capture}.js, ${capture}.scss, ${capture}.css",
    "*.yaml": "*.yml",
    "tailwind.config.*": "tailwind.config*, postcss.config*",
    "tsconfig.json": "tsconfig*",
    "package.json": ".eslint*, .prettier*, package-lock*, pnpm-*, bun.lockb, vite*",
    "appsettings.json": "appsettings*.json, connection*",
    "docker-compose*": "docker-compose*",
    "Dockerfile": "Dockerfile*, .dockerignore",
    "README.md": "*.md, LICENSE",
    ".gitattributes": ".gitmodules, .gitignore"
  },

  // * diffEditor Configs
  "diffEditor.hideUnchangedRegions.enabled": true,
  "diffEditor.ignoreTrimWhitespace": true,
  "diffEditor.renderSideBySide": true,
  "diffEditor.wordWrap": "on",
  "diffEditor.renderIndicators": true,

  // * Git Configs
  "git.openRepositoryInParentFolders": "always",
  "git.decorations.enabled": true,

  // * Other Configs
  "breadcrumbs.enabled": false,
  "window.commandCenter": false,
  "extensions.ignoreRecommendations": true,

  // * Configs for Themes
  "workbench.colorTheme": "One Dark Pro Monokai Darker",
  "theme-by-language.themes": {
    "*": "One Dark Pro Monokai Darker",
    "filename:COMMIT_EDITMSG": "Default Dark Modern",
  },

  // * Configs for Prettier
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

  // * Configs for ESLint
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": "explicit"
  },
  "eslint.validate": [
    "javascript",
    "typescript",
    "vue",
    "graphql"
  ],

  // * Configs for JavaScript
  "javascript.suggest.autoImports": true,
  "javascript.updateImportsOnFileMove.enabled": "always",
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
  "javascript.preferences.organizeImports": {
    "groups": [
      "module",
      "builtin",
      "type",
      "parent",
      "sibling",
      "internal",
      "style"
    ],
    "sortOnBeforeOrganize": true
  },

  // * Configs for TypeScript
  "typescript.tsserver.log": "off",
  "typescript.suggest.autoImports": true,
  "typescript.updateImportsOnFileMove.enabled": "always",
  "typescript.preferences.preferTypeOnlyAutoImports": true,
  "typescript.preferences.jsxAttributeCompletionStyle": "auto",
  "typescript.preferences.importModuleSpecifier": "relative",
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
  "typescript.preferences.organizeImports": {
    "groups": [
      "module",
      "builtin",
      "type",
      "parent",
      "sibling",
      "internal",
      "style"
    ],
    "sortOnBeforeOrganize": true
  },

  // * Configs for Emmet
  "emmet.includeLanguages": {
    "javascript": "javascriptreact",
    "typescript": "typescriptreact"
  },
  "emmet.syntaxProfiles": {
    "javascript": "jsx",
    "typescriptreact": "tsx"
  },

  // * Configs for Vetur
  "vetur.validation.template": false,
  "vetur.validation.style": true,
  "vetur.validation.script": true,
  "vetur.format.defaultFormatter.html": "prettyhtml",
  "vetur.format.defaultFormatter.js": "prettier-eslint",
  "vetur.format.defaultFormatterOptions": {
    "js-beautify-html": {
      "wrap_attributes": "force-aligned"
    },
    "prettyhtml": {
      "printWidth": 100,
      "singleQuote": false,
      "wrapAttributes": false,
      "sortAttributes": false
    },
    "css": {
    "indent_size": 2
    },
    "scss": {
      "indent_size": 2
    }
  },

  // * Configs for Prisma
  "[prisma]": {
    "editor.formatOnSave": true
  },

  // * Configs for Code Runner
  "code-runner.runInTerminal": true,
  "code-runner.enableAppInsights": false,

  // * Configs for UMLet
  "umlet.theme": "Light theme",
  "[umlet]": {
    "files.autoSave": "onFocusChange",
  },

  // * Configs for Symbols
  "symbols.hidesExplorerArrows": false,
  "workbench.iconTheme": "symbols",
  "symbols.files.associations": {
    "*.uxf": "drawio",
    "*.txt": "text"
  },
  "symbols.folders.associations": {
    "controllers": "folder-app",
    "migrations": "folder-database",
    "data": "folder-context",
    "dto": "folder-yellow",
    "requests": "folder-green",
    "responses": "folder-sky",
    "tests": "folder-orange",
    "properties": "folder-gray-outline",
    "configurations": "folder-config",
    "services": "folder-target",
    "views": "folder-layout",
    "repositories": "folder-database",
    "mappers": "folder-router",
    "filters": "folder-purple-outline",
    "logging": "folder-gray",
    "extensions": "folder-red-outline"
  },

  // * Configs for YAML
  "yaml.format.enable": true,
  "yaml.format.singleQuote": false,
  "[yaml]": {
    "editor.formatOnSave": true,
    "editor.autoIndent": "keep",
    "diffEditor.ignoreTrimWhitespace": false,
    "editor.quickSuggestions": {
      "other": true,
      "comments": false,
      "strings": true
    }
  },

  // * Configs for Code Spell Checker
  "cSpell.language": "en,pt,pt_BR",
}
```
