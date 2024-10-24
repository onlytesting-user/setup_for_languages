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

  // * Files Configs
  "files.eol": "\n",
  "files.autoSave": "afterDelay",
  "files.trimTrailingWhitespace": true,
  "files.insertFinalNewline": true,
  "files.associations": {
    "*.cs": "csharp",
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
    "*.cs": "*.csproj",
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
  "search.followSymlinks": false,

  // * Configs for Themes
  "workbench.colorTheme": "One Dark Pro Monokai Darker",
  "theme-by-language.themes": {
    "*": "One Dark Pro Monokai Darker",
    "filename:COMMIT_EDITMSG": "Default Dark Modern",
  },

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

  // * Configs for Code Runner
  "code-runner.runInTerminal": true,
  "code-runner.executorMap": {
    "csharp": "cd $dir && dotnet run",
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
