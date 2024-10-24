# VS Code Configs

```markdown
{
 // * Editor Configs
 "editor.fontFamily": "JetBrains Mono",
 "editor.fontLigatures": true,
 "editor.fontSize": 15,
 "editor.lineHeight": 1.5,
 "editor.rulers": [
  100
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
 "editor.tabSize": 4,
 "editor.indentSize": "tabSize",
 "editor.snippetSuggestions": "top",
 "editor.tabCompletion": "on",
 "editor.quickSuggestions": {
  "other": "on",
  "comments": "off",
  "strings": "off"
 },

 // * Configs for Python
 "[python]": {
    "editor.rulers": [79],
    "editor.defaultFormatter": "ms-python.autopep8",
    "editor.formatOnSave": true,
    "editor.codeActionsOnSave": {
        "source.organizeImports": "explicit"
    },
  },
  "isort.args": ["--profile", "black"],
  "autopep8.args": [
      "--max-line-length", "79",
      "--aggressive",
      "--aggressive"
  ],

  // * Configs for Pylance
  "python.languageServer": "Pylance",
  "python.analysis.typeCheckingMode": "basic",
  "python.analysis.diagnosticMode": "workspace",
  "python.analysis.inlayHints.functionReturnTypes": true,
  "python.analysis.logLevel": "Information",
  "python.analysis.autoFormatStrings": true,

  // * Files Configs
  "files.eol": "\n",
  "files.autoSave": "afterDelay",
  "files.trimTrailingWhitespace": true,
  "files.insertFinalNewline": true,
  "files.associations": {
    "*.py": "python",
    "*.md": "markdown",
    "*.json": "jsonc",
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
  "explorer.autoReveal": false,
  "explorer.confirmDelete": false,
  "explorer.confirmDragAndDrop": false,
  "explorer.sortOrder": "foldersNestsFiles",
  "explorer.compactFolders": false,
  "explorer.fileNesting.enabled": true,
  "explorer.fileNesting.patterns": {
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

  // * Configs for Symbols
  "symbols.hidesExplorerArrows": false,
  "workbench.iconTheme": "symbols",
  "symbols.files.associations": {
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
