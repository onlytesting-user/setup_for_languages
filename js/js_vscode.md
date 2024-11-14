# VS Code Configs

```json
{
  // * Editor Configs
  "editor.fontFamily": "JetBrains Mono",
  "editor.fontLigatures": true,
  "editor.fontSize": 15,
  "editor.lineHeight": 1.5,
  "editor.rulers": [
    120
  ],
  "editor.semanticHighlighting.enabled": true,
  "editor.minimap.enabled": false,
  "editor.accessibilitySupport": "off",
  "editor.suggestSelection": "first",
  "editor.acceptSuggestionOnCommitCharacter": false,
  "editor.stickyScroll.enabled": false,
  "editor.cursorBlinking": "expand",
  "editor.cursorSmoothCaretAnimation": "on",
  "editor.codeLens": true,
  "editor.glyphMargin": true,
  "editor.insertSpaces": true,
  "editor.tabSize": 2,
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
    "*.jsx": "javascriptreact",
    "*.ts": "typescript",
    "*.tsx": "typescriptreact",
    "*.json": "jsonc",
    "*.prettierrc*": "json",
    "*.html": "html",
    "*.css": "css",
    "*.scss": "scss",
    "*.md": "markdown",
    "*.prisma": "prisma",
    "*.yaml": "yaml",
    ".env": "dotenv",
    "Dockerfile": "dockerfile",
    "docker-compose": "dockercompose",
    ".gitignore": "ignore",
    ".dockerignore": "ignore"
  },
  "files.exclude": {
    "**/.git": true,
    "**/.svn": true,
    "**/.hg": true,
    "**/CVS": true,
    "**/.DS_Store": true,
    "**/Thumbs.db": true,
    "**/node_modules": true,
    "**/dist": true,
    "**/.cache": true
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
  "explorer.autoReveal": false,
  "explorer.confirmDelete": false,
  "explorer.confirmDragAndDrop": false,
  "explorer.sortOrder": "foldersNestsFiles",
  "explorer.compactFolders": false,
  "explorer.fileNesting.enabled": true,
  "explorer.fileNesting.patterns": {
    "*.ts": "${capture}.js, ${capture}.test.ts, ${capture}.spec.ts, tsconfig.json",
    "*.js": "${capture}.js.map, ${capture}.min.js, ${capture}.d.ts, ${capture}.test.js, ${capture}.spec.js",
    "*.tsx": "${capture}.ts, ${capture}.test.tsx, ${capture}.spec.tsx, ${capture}.map",
    "*.jsx": "${capture}.js, ${capture}.test.jsx, ${capture}.spec.jsx. ${capture}.map",
    "*.scss": "${capture}.css, ${capture}.min.css, ${capture}.tailwind.css",
    "*.css": "${capture}.min.css, ${capture}.map.css, ${capture}.tailwind.css",
    "tailwind.config.*": "tailwind.config*, postcss.config*",
    "tsconfig.json": "tsconfig*",
    "package.json": ".eslint*, .prettier*, package-lock*, yarn.lock, pnpm-*, vite*",
    "*.yaml": "*.yaml, *.yml",
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
  "search.followSymlinks": false,

  // * Configs for Themes
  "workbench.colorTheme": "One Dark Pro Monokai Darker",
  "theme-by-language.themes": {
    "*": "One Dark Pro Monokai Darker",
    "filename:COMMIT_EDITMSG": "Default Dark Modern",
  },

  // * Configs for Prettier
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "prettier.printWidth": 120,
  "prettier.tabWidth": 2,
  "prettier.useTabs": false,
  "prettier.endOfLine": "lf",
  "prettier.proseWrap": "always",
  "prettier.trailingComma": "es5",
  "prettier.semi": true,
  "prettier.singleQuote": true,
  "prettier.arrowParens": "always",
  "prettier.bracketSpacing": true,

  // * Format on Save
  "[html]": {
    "editor.formatOnSave": true
  },
  "[css]": {
    "editor.formatOnSave": true
  },
  "[scss]": {
    "editor.formatOnSave": true
  },
  "[markdown]": {
    "editor.formatOnSave": true
  },

  // * Configs for ESLint
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": "explicit"
  },
  "eslint.validate": [
    "javascript",
    "javascriptreact",
    "typescript",
    "typescriptreact",
    "graphql",
    "html",
    "css",
    "scss",
    "json"
  ],
  "eslint.options": {
    "configFile": ".eslintrc.js"
  },

  // * Configs for JavaScript
  "javascript.suggest.autoImports": true,
  "javascript.updateImportsOnFileMove.enabled": "always",
  "javascript.preferences.importModuleSpecifier": "project-relative",
  "javascript.suggest.completeFunctionCalls": true,
  "[javascript]": {
    "editor.formatOnSave": true,
    "editor.snippetSuggestions": "top",
    "editor.tabCompletion": "on",
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
  "sortOnBeforeOrganize": true,
  "javascript.preferences.organizeImports": {
    "groups": [
      "module",
      "builtin",
      "type",
      "parent",
      "sibling",
      "internal",
      "style"
    ]
  },

  // * Configs for TypeScript
  "typescript.tsserver.log": "normal",
  "typescript.suggest.autoImports": true,
  "typescript.updateImportsOnFileMove.enabled": "always",
  "typescript.preferences.preferTypeOnlyAutoImports": true,
  "typescript.preferences.importModuleSpecifier": "project-relative",
  "typescript.preferences.includePackageJsonAutoImports": "on",
  "typescript.preferences.importModuleSpecifierEnding": "auto",
  "typescript.suggest.completeFunctionCalls": true,
  "typescript.preferences.jsxAttributeCompletionStyle": "braces",
  "[typescript]": {
    "editor.formatOnSave": true,
    "editor.snippetSuggestions": "top",
    "editor.tabCompletion": "on",
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
  "sortOnBeforeOrganize": true,
  "typescript.preferences.organizeImports": {
    "groups": [
      "module",
      "builtin",
      "type",
      "parent",
      "sibling",
      "internal",
      "style"
    ]
  },

  // * Configs for React
  "[javascriptreact]": {
    "editor.formatOnSave": true,
    "editor.snippetSuggestions": "top",
    "editor.tabCompletion": "on",
    "editor.codeActionsOnSave": {
      "source.organizeImports": "explicit",
      "source.fixAll.jsx": "explicit"
    },
    "editor.quickSuggestions": {
      "other": "on",
      "comments": "off",
      "strings": "on"
    }
  },
  "[typescriptreact]": {
    "editor.formatOnSave": true,
    "editor.snippetSuggestions": "top",
    "editor.tabCompletion": "on",
    "editor.codeActionsOnSave": {
      "source.organizeImports": "explicit",
      "source.fixAll.tsx": "explicit"
    },
    "editor.quickSuggestions": {
      "other": "on",
      "comments": "off",
      "strings": "on"
    }
   },

  // * Configs for Emmet
  "emmet.showAbbreviationSuggestions": true,
  "emmet.includeLanguages": {
    "javascript": "javascriptreact",
    "typescript": "typescriptreact"
  },
  "emmet.syntaxProfiles": {
    "javascriptreact": "jsx",
    "typescriptreact": "tsx"
  },

  // * Configs for Prisma
  "[prisma]": {
    "editor.formatOnSave": true,
    "editor.snippetSuggestions": "top"
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
    // Specific Symbols
    "configurations": "folder-config",
    "controllers": "folder-app",
    "data": "folder-context",
    "mappers": "folder-router",
    "migrations": "folder-database",
    "pages": "folder-layout",
    "repositories": "folder-database",
    "security": "folder-auth",
    "services": "folder-target",
    "views": "folder-layout",
    
    // Generic Colors
    "backend": "folder-green",
    "docs": "folder-pink",
    "dto": "folder-yellow",
    "extensions": "folder-red-outline",
    "filters": "folder-purple-outline",
    "frontend": "folder-yellow",
    "logging": "folder-gray",
    "properties": "folder-gray-outline",
    "redux": "folder-pink-code",
    "requests": "folder-red",
    "responses": "folder-sky",
    "tests": "folder-orange",
    "vendor": "folder-purple-code"
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
