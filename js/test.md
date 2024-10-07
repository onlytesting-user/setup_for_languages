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
    "*.jsx": "javascriptreact",
    "*.ts": "typescript",
    "*.tsx": "typescriptreact",
    ".prettierrc": "json",
    "*.html": "html",
    "*.css": "css",
    "*.md": "markdown",
    "*.json": "jsonc",
    "*.prisma": "prisma"
    "*.yaml": "yaml",
    ".env": "dotenv",
  },
  "files.exclude": {
    "**/.git": true,
    "**/.svn": true,
    "**/.hg": true,
    "**/CVS": true,
    "**/.DS_Store": true,
    "**/Thumbs.db": true,
    "**/.vscode": true,
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

  // * Explorer Configs
  "explorer.confirmDelete": false,
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
    "appsettings.json": "appsettings*.json, connection*",
    "docker-compose*": "docker-compose*, .docker-compose*",
    "Dockerfile": "Dockerfile*, .dockerignore",
    "README.md": "*.md, LICENSE",
    ".gitattributes": ".gitmodules, .gitignore",
  },

  // * Update Configs
  "update.mode": "default",
  "update.showReleaseNotes": false,

  // * diffEditor Configs
  "diffEditor.hideUnchangedRegions.enabled": true,
  "diffEditor.ignoreTrimWhitespace": true,
  "diffEditor.renderSideBySide": true,
  "diffEditor.wordWrap": "on",
  "diffEditor.renderIndicators": true,

  // * Git Configs
  "git.openRepositoryInParentFolders": "always",
  "git.decorations.enabled": true,

  // * Security Configs
  "security.workspace.trust.untrustedFiles": "newWindow",
  "security.promptForLocalFileProtocolHandling": true,

  // * Other Configs
  "breadcrumbs.enabled": false,
  "window.commandCenter": false,
  "extensions.ignoreRecommendations": true,
  "extensions.autoCheckUpdates": true,

  // * Configs for Themes
  "workbench.colorTheme": "One Dark Pro Monokai Darker",

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
  }, // NOTE Retirar se decidir não usar React
  "emmet.syntaxProfiles": {
    "javascript": "jsx"
  }, // NOTE Retirar se decidir não usar React
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
    "Controllers": "folder-app",
    "Migrations": "folder-database",
    "Data": "folder-context",
    "Dto": "folder-yellow",
    "Requests": "folder-green",
    "Responses": "folder-sky",
    "Tests": "folder-orange",
    "Properties": "folder-gray-outline",
    "Configurations": "folder-config",
    "Services": "folder-target",
    "Views": "folder-layout",
    "Repositories": "folder-database",
    "Mappers": "folder-router",
    "Filters": "folder-purple-outline",
    "Logging": "folder-gray",
    "Extensions": "folder-red-outline"
  },

  // * Configs for YAML
  "yaml.format.enable": true,
  "yaml.format.singleQuote": true,
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
  "cSpell.userWords": [

  ],
}
```
