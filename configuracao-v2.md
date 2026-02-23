# 👨🏼‍💻 Nova configuração do VSCode

📍 Sumário

- [`Plugins`](#plugins)
- [`Thema`](#thema)
- [`Configuração`](#configuração)
- [`Custom CSS do Plugin (Custom CSS and JS Loader)`](#custom-css)

## Plugins

1. `Bookmarks`
2. `Bracket Pair Color DLW`
3. `Codex – OpenAI’s coding agent`
4. `CSS Peek`
5. `Custom CSS and JS Loader`
6. `Error Gutters`
7. `Error Lens`
8. `ESLint`
9. `Fluent Icons`
10. `Live Preview`
11. `Live Sass Compiler`
12. `Material Icon Theme`
13. `Min Theme`
14. `Monokai Pro`
15. `Path Intellisense`
16. `PHP Intelephense`
17. `Prettier - Code formatter`
18. `Tailwind CSS IntelliSense`
19. `VSLook`

## Thema

- Thema Clonado: Monokai Pro (Filter Spectrum)
- Clonado pelo o plugin VSLook
- Verificar arquivo do thema do vslook para download

## Configuração

`settings.json`

```json
{
  "workbench.iconTheme": "material-icon-theme",
  "workbench.productIconTheme": "fluent-icons",
  "workbench.tips.enabled": false,
  "workbench.tree.renderIndentGuides": "none",
  "workbench.startupEditor": "newUntitledFile", // Abre uma nova tela vazia.
  "workbench.editor.labelFormat": "short",

  // Associação do Material Icons
  "material-icon-theme.folders.associations": {
    "infra": "app",
    "entities": "class",
    "schemas": "class",
    "typeorm": "database",
    "migrations": "tools",
    "modules": "components",
    "implementations": "core",
    "dtos": "typescript",
    "fakes": "mock",
    "languageId": "iconName",
    "json": "json",
    "backend": "server",
  },

  "material-icon-theme.files.associations": {
    "*.ts": "typescript",
    "**.json": "json",
    "fileName.ts": "angular",
  },

  "material-icon-theme.languages.associations": {
    "languageId": "iconName",
    "json": "json",
  },
  //

  // Mostrar as arrows nas pastas
  "material-icon-theme.hidesExplorerArrows": false,

  // Tailwind
  "files.associations": {
    "*.css": "tailwindcss",
  },

  "tailwindCSS.includeLanguages": {
    "html": "html",
    "javascript": "javascript",
    "javascriptreact": "javascriptreact",
    "typescript": "typescript",
    "typescriptreact": "typescriptreact",
    "php": "html",
  },

  // Colorização Brackets
  "editor.bracketPairColorization.enabled": true,
  "editor.guides.bracketPairs": "active",
  "editor.guides.indentation": true,

  // Prettier (global)
  "editor.defaultFormatter": "esbenp.prettier-vscode",

  "prettier.prettierPath": "./node_modules/prettier",

  // ESLint só quando você executar explicitamente (não briga com Prettier no save)
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": "explicit",
  },

  // Prettier - defaults globais (otimizado p/ HTML + PHP)
  "prettier.requireConfig": false,
  "prettier.printWidth": 160,
  "prettier.tabWidth": 2,
  "prettier.useTabs": false,
  "prettier.semi": true,
  "prettier.singleQuote": true,
  "prettier.trailingComma": "es5",
  "prettier.bracketSpacing": true,
  "prettier.arrowParens": "avoid",
  "prettier.proseWrap": "never",

  // HTML (reduz quebras e “tag sozinha”)
  "prettier.htmlWhitespaceSensitivity": "ignore",
  "prettier.bracketSameLine": true,
  "prettier.singleAttributePerLine": false,

  "[php]": { "editor.defaultFormatter": "bmewburn.vscode-intelephense-client" },
  "[html]": { "editor.defaultFormatter": "esbenp.prettier-vscode" },
  "[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode",
  },

  // Opcional/redundante, mas deixa explícito por linguagem

  "[twig]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode",
  },

  // Editor
  "editor.linkedEditing": true,
  "editor.wordWrap": "on",
  "editor.fontSize": 14,
  "editor.fontFamily": "JetBrains Mono",
  "window.commandCenter": false,
  "editor.lineHeight": 1.8,
  "editor.fontLigatures": true,
  "editor.fontVariations": false,
  "editor.formatOnSave": true,

  "editor.renderLineHighlight": "none",
  "editor.semanticHighlighting.enabled": false,
  "editor.scrollbar.horizontal": "hidden",
  "editor.scrollbar.vertical": "hidden",

  "editor.hideCursorInOverviewRuler": true,
  "editor.renderWhitespace": "none",
  "editor.matchBrackets": "never",
  "editor.lightbulb.enabled": "off",
  "editor.hover.enabled": "on",

  "editor.showFoldingControls": "mouseover",
  "editor.foldingHighlight": false,
  "editor.overviewRulerBorder": false,
  "editor.cursorSmoothCaretAnimation": "on",
  "editor.cursorBlinking": "smooth",
  "editor.detectIndentation": true,
  "editor.parameterHints.enabled": false,
  "window.newWindowProfile": "Default",

  // Explorer
  "explorer.confirmDragAndDrop": false,
  "explorer.confirmDelete": false,
  "explorer.compactFolders": true,

  "breadcrumbs.enabled": false,

  // Git
  // "git.decorations.enabled": false,

  // Live Sass Compiler
  "liveSassCompile.settings.autoprefix": [],
  "liveSassCompile.settings.formats": [
    {
      "format": "compressed",
      "extensionName": ".min.css",
      "savePath": "/assets/css",
    },
  ],

  // Outros
  "html.completion.attributeDefaultValue": "doublequotes",

  // Terminal
  "terminal.integrated.fontFamily": "JetBrains Mono NL",
  "terminal.integrated.fontLigatures.enabled": true,
  "terminal.integrated.fontSize": 14,
  "terminal.integrated.lineHeight": 1.3,
  "terminal.integrated.scrollback": 10000,
  "terminal.integrated.cursorBlinking": true,
  "terminal.integrated.cursorStyle": "line",
  "terminal.integrated.cursorWidth": 2,

  "scm.diffDecorations": "none",
  "files.insertFinalNewline": true,

  "emmet.syntaxProfiles": {
    "javascript": "jsx",
  },

  // Javascript
  "typescript.tsserver.log": "off",

  "files.exclude": {
    "**/.git": true,
    "**/.svn": true,
    "**/.hg": true,
    "**/.DS_Store": true,
    "**/Thumbs.db": true,
    "**/CVS": true,
    "node_modules": true,
  },

  "zenMode.fullScreen": false,
  "zenMode.centerLayout": false,
  "zenMode.showTabs": "single",

  // Não abrir o terminal ao salvar no sass
  "liveSassCompile.settings.showOutputWindowOn": "None",
  "git.confirmSync": false,

  "php.validate.executablePath": "/Applications/MAMP/bin/php/php8.3.28/bin/php",
  "workbench.colorTheme": "VSLook",
  // "material-icon-theme.opacity": 0.5,

  // // Customizando o Tema
  // "editor.tokenColorCustomizations": {
  //   "textMateRules": [
  //     {
  //       "name": "HTML tag names (incl. DOCTYPE)",
  //       "scope": ["entity.name.tag.html", "entity.name.tag", "meta.tag.metadata.doctype.html"],
  //       "settings": {
  //         "foreground": "#FC618D",
  //       },
  //     },
  //   ],
  // },

  // "workbench.colorCustomizations": {
  //   "editor.background": "#111114",
  //   "editorGutter.background": "#111114",
  // },

  // Origamid
  "editor.glyphMargin": false,
  "editor.hover.delay": 125,
  "editor.hover.hidingDelay": 125,
  "scm.diffDecorationsGutterVisibility": "hover",

  "vscode_custom_css.imports": ["file:///Users/renatojunior/Documents/custom-vscode/custom.css"],
  "settingsSync.ignoredSettings": [],
  "vslook.palette.colors": {
    "base": {
      "fundo-1": "#202020",
      "amarelo": "#f7e164",
      "editor-1": "#19191a",
      "sidebar-1": "#111114",
    },
  },

  "editor.inlineSuggest.enabled": true,
  "editor.quickSuggestions": {
    "other": "on",
    "comments": "off",
    "strings": "on",
  },

  "livePreview.autoRefreshPreview": "On Changes to Saved Files",
  "livePreview.portNumber": 5000,
  "livePreview.previewDebounceDelay": 0,
  "workbench.activityBar.location": "top",
  
  // A IDE não fixar a tag pai no scroll
  "editor.stickyScroll.enabled": false,
}

```

## Custom CSS

`custom.css`

```css
.composite-bar-container {
    padding-left: 8px;
}

.tabs-container {
    margin-bottom: 6px;
    padding: 6px;
}

.monaco-workbench .pane-composite-part>.header-or-footer {
    padding-left: 4px;
    padding-right: 4px;
    background-color: #111114;
}

```
Após adicionar, usar o ctrl + shift + p e procurar por `Enable Custom CSS and JS` o vscode vai pedir para reiniciar e após isso, ele vai ativar as configurações.