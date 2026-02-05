# Especificações
Configurações do meu vscode para mac/windows

## Plugins que uso
- ACF-Snippet
- Beautify css/sass/scss/less
- Bookmarks
- cdnjs
- CodeSnap
- Codex – OpenAI’s coding agent
- Container Tools
- CSS Peek
- Custom CSS and JS Loader
- Docker
- Docker DX
- Elementor Snippets & Autocompletions
- Error Gutters
- Error Lens
- ESLint
- Fluent Icons
- Format HTML in PHP
- GitHub Copilot Chat
- GitLens — Git supercharged
- JavaScript (ES6) code snippets
- jQuery Code Snippets
- Live Sass Compiler
- Live Preview
- Markdown Preview Enhanced
- Material Icon Theme
- Monokai Pro
- Node.js Exec
- Path Intellisense
- PHP IntelliSense
- Pixel To Rem Converter
- Prettier - Code formatter
- Rainbow CSV
- Remote - SSH
- Remote - SSH: Editing Configuration Files
- Remote - Tunnels
- Remote Explorer
- Svg Preview
- vscode-pdf
- VSLook
- WordPress Snippets
- GitHub Copilot

### Tema 1 / Default
#### settings.json

```json
{
    // workbench
    "workbench.productIconTheme": "fluent-icons",
    "workbench.iconTheme": "material-icon-theme",
    "workbench.colorTheme": "VSLook",
    "workbench.tips.enabled": false,
    "workbench.statusBar.visible": true,
    "workbench.tree.renderIndentGuides": "none",

    // Editor
    "editor.linkedEditing": true,
    "editor.wordWrap": "on",
    "editor.fontSize": 15,
    "editor.fontFamily": "JetBrains Mono",
    "editor.lineHeight": 1.9,
    "editor.fontLigatures": true,
    "editor.fontVariations": false,
    "editor.formatOnSave": true,
    "editor.renderLineHighlight": "none",
    "editor.semanticHighlighting.enabled": false,
    "editor.scrollbar.horizontal": "hidden",
    "editor.scrollbar.vertical": "hidden",
    "editor.hideCursorInOverviewRuler": true,
    "editor.guides.indentation": true,
    "editor.renderWhitespace": "none",
    "editor.matchBrackets": "never",
    "editor.lightbulb.enabled": "off",
    "editor.hover.enabled": "off",
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

    // Git
    "git.decorations.enabled": false,

    // Live Sass Compiler
    "liveSassCompile.settings.autoprefix": [],
    "liveSassCompile.settings.formats": [
        {
            "format": "compressed",
            "extensionName": ".min.css",
            "savePath": "/assets/css",
        },
    ],

    // Live Server
    "liveServer.settings.donotShowInfoMsg": true,

    // Outros
    "window.commandCenter": false,
    "html.completion.attributeDefaultValue": "doublequotes",
    "html.format.indentHandlebars": true,
    "html.format.indentInnerHtml": true,
    "pixelToRem.pixelValue": 10,
    "extensions.ignoreRecommendations": true,
    "explorer.compactFolders": false,
    "breadcrumbs.enabled": false,
    "[css]": {
        "editor.defaultFormatter": "michelemelluso.code-beautifier",
    },
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
    "[html]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode",
    },
    "emmet.syntaxProfiles": {
        "javascript": "jsx",
    },

    // Prettier
    "prettier.tabWidth": 4,

    "security.workspace.trust.untrustedFiles": "open",

    // Javascript
    "javascript.suggest.autoImports": true,
    "javascript.updateImportsOnFileMove.enabled": "always",
    "typescript.tsserver.log": "off",

    "files.associations": {
        ".sequelizerc": "javascript",
        ".stylelintrc": "json",
        "*.tsx": "typescriptreact",
        ".env.*": "dotenv",
        ".prettierrc": "json",
    },
    "files.exclude": {
        "**/.git": true,
        "**/.svn": true,
        "**/.hg": true,
        "**/.DS_Store": true,
        "**/Thumbs.db": true,
        "**/CVS": true,
        "node_modules": true,
    },

    "emmet.includeLanguages": {
        "javascript": "javascriptreact",
    },

    // Preset do Maykão
    "editor.glyphMargin": false,
    "files.autoSaveDelay": 1500,

    // Zen mode
    "zenMode.fullScreen": false,
    "zenMode.centerLayout": false,
    "zenMode.showTabs": "single",

    // Preset do Diego da Rockeatseat
    "workbench.startupEditor": "newUntitledFile",
    "workbench.editor.labelFormat": "short",
    "explorer.fileNesting.enabled": true,
    "explorer.fileNesting.patterns": {
        "*.ts": "${capture}.js",
        "*.js": "${capture}.js.map, ${capture}.min.js, ${capture}.d.ts",
        "*.jsx": "${capture}.js",
        "*.tsx": "${capture}.ts",
        "tsconfig.json": "tsconfig.*.json",
        "package.json": "package-lock.json, yarn.lock, pnpm-lock.yaml, bun.lockb, bun.lock",
    },

    // Não abrir o terminal ao salvar no sass
    "liveSassCompile.settings.showOutputWindowOn": "None",
    "git.confirmSync": false,

    // CSS Customizado do vscode
    "vscode_custom_css.imports": [
        "file:///Users/renatojunior/Documents/custom-vscode.css",
    ],
    "settingsSync.ignoredSettings": [],
    "vslook.palette.colors": {
        "base": {
            "neon": "#09ecf8",
            "dark 2": "#191c1f",
            "borda": "hsl(197, 11%, 12%)",
            "item_transparent": "hsl(219, 16%, 21%)",
            "amarelo": "#fce566",
            "border_light": "hsl(51, 97%, 35%)",
            "cor original": "#222222",
            "atributo_1": "#c792ea",
            "aside": "#121517",
            "opacidade-0.2": "rgba(255, 255, 255, 0.2)",
            "green": "#aefe06",
        },
    },
    "gitlens.ai.model": "vscode",
    "gitlens.ai.vscode.model": "copilot:gpt-4o-mini",
    "git.autofetch": true,
    "docker.extension.dockerEngineAvailabilityPrompt": false,
    "github.copilot.enable": {
        "*": true,
        "plaintext": false,
        "markdown": false,
        "scminput": false,
        "scss": false,
        "php": false,
    },
    "markdown-preview-enhanced.codeBlockTheme": "auto.css",
    "chat.mcp.gallery.enabled": true,
    "php.validate.executablePath": "/Applications/MAMP/bin/php/php8.3.28/bin/php",

    "editor.defaultFormatter": "esbenp.prettier-vscode",
    "[javascript]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode",
    },
    "git.enableSmartCommit": true,

    "workbench.activityBar.location": "top",
}

```

### Tema 2 / Origamid

#### Plugins

- Bookmarks
- Live Preview
- Material Icon Theme
- Origamid Next
- Prettier - Code formatter
- Tailwind CSS IntelliSense

#### settings.json

```json
{
    "workbench.colorTheme": "Origamid Next Future",
    "workbench.iconTheme": "material-icon-theme",
    "accessibility.verbosity.hover": false,
    "breadcrumbs.enabled": false,
    "css.hover.references": false,
    "diffEditor.ignoreTrimWhitespace": false,
    "diffEditor.renderSideBySide": true,
    "editor.acceptSuggestionOnEnter": "on",
    "editor.accessibilitySupport": "off",
    "editor.autoClosingBrackets": "always",
    "editor.autoClosingQuotes": "always",
    "editor.bracketPairColorization.enabled": false,
    "editor.colorDecoratorsActivatedOn": "click",
    "editor.defaultColorDecorators":"always",
    "editor.definitionLinkOpensInPeek": false,
    "editor.fontFamily": "JetBrains Mono, Courier New",
    "editor.fontSize": 15,
    "editor.formatOnSave": true,
    "editor.glyphMargin": false,
    "editor.hover.delay": 125,
    "editor.hover.hidingDelay": 125,
    "editor.inlineSuggest.enabled": true,
    "editor.lineHeight": 28,
    "editor.hideCursorInOverviewRuler": true,
    "editor.quickSuggestions": {
        "other": "on",
        "comments": "off",
        "strings": "on"
    },
    "editor.quickSuggestionsDelay": 0,
    "editor.rename.enablePreview": false,
    "editor.renderWhitespace": "selection",
    "editor.scrollbar.horizontal": "hidden",
    "editor.snippetSuggestions": "inline",
    "editor.stickyScroll.enabled": false,
    "editor.suggest.snippetsPreventQuickSuggestions": false,
    "editor.suggestOnTriggerCharacters": true,
    "editor.suggestSelection": "first",
    "editor.tabCompletion": "on",
    "editor.wordWrap": "on",
    
    // Linha marcadora do cursor atual
    "editor.renderLineHighlight": "none",
    "explorer.confirmDragAndDrop": false,
    "explorer.sortOrder": "default",
    "git.enabled": true,
    "git.openRepositoryInParentFolders": "never",
    "html.autoClosingTags": false,
    "html.format.wrapAttributes": "auto",
    "html.format.wrapAttributesIndentSize": 0,
    "html.hover.documentation": false,
    "html.hover.references": false,
    "[html]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "livePreview.autoRefreshPreview": "On Changes to Saved Files",
    "livePreview.portNumber": 5000,
    "livePreview.previewDebounceDelay": 0,
    "prettier.printWidth": 80,
    "prettier.singleQuote": true,
    "prettier.trailingComma": "all",
    "scm.diffDecorationsGutterVisibility": "hover",
    "terminal.integrated.fontSize": 15,
    "window.title": "${activeEditorMedium}${separator}${rootName}",
    "workbench.activityBar.location": "top",    
    "workbench.editor.empty.hint": "hidden",
    "workbench.startupEditor": "newUntitledFile",
    "workbench.statusBar.visible": false,

    // Customização
    "workbench.colorCustomizations": {
        "activityBar.background":"#111114",
        "activityBar.border":"#111114",
        "activityBar.foreground":"#88888b",
        "activityBarBadge.background":"#88dd33",
        "activityBarBadge.foreground":"#222225",

        "badge.background":"#88dd33",
        "badge.foreground":"#222225",
        "button.background":"#333336",
        "button.foreground":"#cccccf",
        "button.hoverBackground":"#222225",

        "debugExceptionWidget.background":"#333336",
        "debugExceptionWidget.border":"#222225",
        "debugToolBar.background":"#111114",
        "diffEditor.insertedTextBackground":"#ffdd440c",
        "diffEditor.insertedTextBorder":"#ffdd44",
        "diffEditor.removedTextBackground":"#88bbff00",
        "diffEditor.removedTextBorder":"#77ccff",
        "dropdown.background":"#222225",
        "dropdown.border":"#222225",
        "dropdown.foreground":"#88888b",

        "editor.background":"#19191b",
        "editor.findMatchBackground":"#44444788",
        "editor.findMatchHighlightBackground":"#444447aa",
        "editor.foreground":"#ffffff",
        "editor.hoverHighlightBackground":"#44444788",
        "editor.inactiveSelectionBackground":"#44444788",
        "editor.lineHighlightBackground":"#00000066",
        "editor.lineHighlightBorder":"#00000000",
        "editor.rangeHighlightBackground":"#333336cc",
        "editor.selectionBackground":"#555558",
        "editor.selectionForeground":"#ffffff",
        "editor.selectionHighlightBackground":"#33333688",
        "editor.wordHighlightBackground":"#44444788",
        "editor.wordHighlightStrongBackground":"#44444788",
        "editorBracketMatch.background":"#222225",
        "editorBracketMatch.border":"#666669",
        "editorCodeLens.foreground":"#666669",
        "editorCursor.foreground":"#ffffff",
        "editorError.foreground":"#ee5500",
        "editorGroup.border":"#111114",
        "editorGroup.dropBackground":"#111114bb",
        "editorGroupHeader.noTabsBackground":"#111114",
        "editorGroupHeader.tabsBorder":"#000000",
        "editorGutter.addedBackground":"#ffdd44",
        "editorGutter.background":"#18181b",
        "editorGutter.deletedBackground":"#77ccff",
        "editorGutter.modifiedBackground":"#77ccff",
        "editorHoverWidget.background":"#313134",
        "editorHoverWidget.border":"#000000",
        "editorHoverWidget.foreground":"#cccccf",
        "editorIndentGuide.activeBackground1": "#1C1C1F",
        "editorIndentGuide.background1": "#1C1C1F",
        "editorLineNumber.foreground": "#333336",
        "editorLineNumber.activeForeground": "#88888B",
        "editorLink.activeForeground": "#AA99FF",
        "editorMarkerNavigation.background": "#333336",
        "editorMarkerNavigationError.background":"#77ccff",
        "editorMarkerNavigationWarning.background": "#77CCFF",
        "editorOverviewRuler.addedForeground": "#FFDD44",
        "editorOverviewRuler.border": "#222225",
        "editorOverviewRuler.currentContentForeground": "#333336",
        "editorOverviewRuler.deletedForeground": "#77CCFF",
        "editorOverviewRuler.errorForeground": "#77CCFF",
        "editorOverviewRuler.findMatchForeground": "#555558CC",
        "editorOverviewRuler.incomingContentForeground": "#333336",
        "editorOverviewRuler.infoForeground": "#AA99FF",
        "editorOverviewRuler.modifiedForeground": "#77CCFF",
        "editorOverviewRuler.rangeHighlightForeground": "#333336CC",
        "editorOverviewRuler.selectionHighlightForeground": "#555558CC",
        "editorOverviewRuler.warningForeground": "#77CCFF",
        "editorOverviewRuler.wordHighlightForeground": "#333336CC",
        "editorOverviewRuler.wordHighlightStrongForeground": "#555558CC",
        "editorRuler.foreground": "#FFFFFF",
        "editorSuggestWidget.background": "#313134",
        "editorSuggestWidget.border": "#000000",
        "editorSuggestWidget.foreground": "#CCCCCF",
        "editorSuggestWidget.highlightForeground": "#FFFFFF",
        "editorSuggestWidget.selectedBackground": "#111114",
        "editorWarning.border": "#000000",
        "editorWarning.foreground": "#77CCFF",
        "editorWhitespace.foreground": "#555558",
        "editorWidget.background":"#313134",
        "editorWidget.border":"#000000",
        "extensionButton.prominentHoverBackground": "#555558",

        "focusBorder": "#555558",
        "foreground": "#FFFFFF",

        "gitDecoration.modifiedResourceForeground": "#CCCCCF",
        "gitDecoration.untrackedResourceForeground": "#CCCCCF",
        "inputValidation.errorBackground": "#333336",
        "inputValidation.errorBorder": "#77CCFF",
        "inputValidation.infoBackground": "#333336",
        "input.background": "#333336",
        "input.border": "#333336",
        "input.foreground": "#FFFFFF",
        "input.placeholderForeground": "#555558",
        "inputOption.activeBorder": "#555558",
        "inputValidation.infoBorder": "#AA99FF",
        "inputValidation.warningBackground": "#333336",
        "inputValidation.warningBorder": "#77CCFF",

        "list.activeSelectionBackground": "#333336",
        "list.activeSelectionForeground": "#FFFFFF",
        "list.dropBackground": "#111114BB",
        "list.focusBackground": "#222225",
        "list.focusForeground": "#FFFFFF",
        "list.highlightForeground": "#FFFFFF",
        "list.hoverBackground": "#333336",
        "list.hoverForeground": "#FFFFFF",
        "list.inactiveSelectionBackground": "#000000",

        "merge.currentHeaderBackground": "#555558CC",
        "merge.incomingContentBackground": "#555558CC",
        "merge.incomingHeaderBackground": "#666669CC",

        "panel.background": "#111114",
        "panel.border": "#000000",
        "panel.title.activeBorder": "#FFFFFF",
        "panelTitle.activeForeground": "#FFFFFF",
        "panelTitle.inactiveForeground": "#88888B",
        "peekView.border": "#222225",
        "peekViewEditor.background": "#333336",
        "peekViewEditor.matchHighlightBackground": "#555558",
        "peekViewEditorGutter.background": "#333336",
        "peekViewResult.fileForeground": "#88888B",
        "peekViewResult.lineForeground": "#88888B",
        "peekViewResult.matchHighlightBackground": "#555558",
        "peekViewResult.selectionBackground": "#333336",
        "peekViewResult.selectionForeground": "#FFFFFF",
        "peekViewTitle.background": "#333336",
        "peekViewTitleDescription.foreground": "#88888B",
        "peekViewTitleLabel.foreground": "#FFFFFF",
        "pickerGroup.border": "#222225",
        "pickerGroup.foreground": "#555558",
        "progressBar.background": "#333336",
        
        "quickInput.background": "#111114",
        "quickInput.foreground": "#FFFFFF",
        "quickInputList.focusBackground": "#333336",
        "quickInputList.focusForeground": "#FFFFFF",
        
        "scrollbar.shadow":"#111114",
        "scrollbarSlider.activeBackground":"#222225",
        "scrollbarSlider.background":"#222225",
        "scrollbarSlider.hoverBackground":"#222225",
        "selection.background": "#111114",
        "sideBar.background": "#111114",
        "sideBar.border": "#000000",
        "sideBar.foreground": "#88888B",
        "sideBarSectionHeader.background": "#111114",
        "sideBarSectionHeader.foreground": "#666669",
        "sideBarTitle.foreground": "#555558",
        "statusBar.background": "#111114",
        "statusBar.border": "#000000",
        "statusBar.debuggingBackground": "#666669",
        "statusBar.debuggingForeground": "#FFFFFF",
        "statusBar.foreground": "#666669",
        "statusBar.noFolderBackground": "#111114",
        "statusBar.noFolderForeground": "#666669",
        "statusBarItem.activeBackground": "#222225",
        "statusBarItem.hoverBackground": "#222225",
        "statusBarItem.hoverForeground": "#FFFFFF",
        "statusBarItem.prominentBackground": "#333336",
        "statusBarItem.prominentHoverBackground": "#444447",
        
        "tab.activeBackground": "#1C1C1F",
        "tab.border": "#000000",
        "tab.inactiveBackground": "#111114",
        "tab.inactiveForeground": "#88888B",
        "tab.unfocusedActiveBorder": "#88888B",
        "tab.unfocusedActiveForeground": "#88888B",
        "tab.unfocusedInactiveForeground": "#88888B",
        "terminal.ansiBlack": "#333336",
        "terminal.ansiBlue": "#77CCFF",
        "terminal.ansiBrightBlack": "#666669",
        "terminal.ansiBrightBlue": "#77CCFF",
        "terminal.ansiBrightCyan": "#AA99FF",
        "terminal.ansiBrightGreen": "#FFDD44",
        "terminal.ansiBrightMagenta": "#77CCFF",
        "terminal.ansiBrightRed": "#77CCFF",
        "terminal.ansiBrightWhite": "#FFFFFF",
        "terminal.ansiBrightYellow": "#88DD33",
        "terminal.ansiCyan": "#AA99FF",
        "terminal.ansiGreen": "#FFDD44",
        "terminal.ansiMagenta": "#77CCFF",      
        "terminal.ansiRed": "#77CCFF",
        "terminal.ansiWhite": "#FFFFFF",
        "terminal.ansiYellow": "#88DD33",
        "terminal.background": "#111114",
        "terminal.foreground": "#FFFFFF",
        "textLink.activeForeground": "#77CCFF",
        "textLink.foreground": "#77CCFF",
        "titleBar.activeBackground": "#111114",
        "titleBar.activeForeground": "#88888B", 
        "titleBar.border":"#00000c",
        "titleBar.inactiveBackground":"#111114",
        "titleBar.inactiveForeground":"#555558",
        "walkThrough.embeddedEditorBackground":"#111114",
        "widget.shadow":"#111114cc"
    },
    "editor.tokenColorCustomizations": {
        "textMateRules": [
            {
                "scope":[
                    "source.js.jsx punctuation.section.embedded",
                    "string.other.link.description.title",
                    "support.constant",
                    "support.variable",
                    "support.type",
                    "support.class.builtin.js",
                    "support.class.console.js",
                    "meta.property-value",
                    "meta.at-rule.keyframes entity.name.function",
                    "expression.embedded.vue punctuation.definition",
                    "entity.name.tag",
                    "entity.other.attribute-name.pseudo-class.css",
                    "entity.other.attribute-name.pseudo-element.css",
                    "entity.name.type.object.console",
                    "variable.parameter.keyframe-list",
                    "variable.other.class",
                    "variable.language",
                    "variable.parameter.function.language.special.self.python",
                    "storage.type",
                    "punctuation.definition.string.template"
                ],
                "settings": {
                    "foreground": "#AA99FF",
                }
            },
            {
                "scope": [
                    "meta.function-call meta.function-call.arguments",
                    "meta.function-call meta.arguments",
                    "meta.function-call meta.group",
                    "source.json meta.structure.dictionary",
                    "meta.object.member",
                    "punctuation.definition.group",
                    "string.unquoted.label",
                    "variable.other.member",
                    "entity.name.class",
                    "entity.name.namespace",
                    "constant.other",
                    "variable",
                    "variable.other",
                    "variable.other.constant.js",
                    "text.find-in-files",
                    "source",
                    "entity.name.type.module",
                    "source.sql support.function",
                    "support.other.namespace.php",
                    "variable.parameter",
                    "parameters variable.function"
                ],
                "settings": {
                    "foreground": "#FFFFFF",                    
                }                   
            },
            {
                "scope": [
                    "variable.other.property",
                    "support.variable.property",
                    "punctuation.separator.key-value",
                    "meta.object-literal.key",
                    "variable.other.object.property",
                    "variable.object.property",
                    "text.html.basic",
                    "text.html.vue-html",
                    "text.html.php",
                    "text.html.derivative",
                    "punctuation.definition.variable",
                    "punctuation.definition.keyword.scss",
                    "meta.jsx.children.js",
                    "meta.tag.attributes keyword.operator.assignment",
                    "support.type.vendored.property-name.css",
                    "support.type.property-name.json",
                    "variable.other.constant.property",
                    "meta.property-name support.type"                    
                ],
                "settings": {
                    "foreground": "#CCCCCF",                    
                }
            },
            {
                "scope": [
                    "keyword.other.substitution",
                    "keyword.operator.heading.restructuredtext",
                    "keyword.operator.table.row.restructuredtext",
                    "keyword.operator.table.data.restructuredtext",
                    "punctuation",
                    "markup.ignored",
                    "markup.untracked",
                    "meta.brace.round",
                    "meta.brace.round",
                    "meta.brace.square",
                    "meta.brace.curly",
                    "meta.delimiter.comma.js",
                    "meta.function-call.without-arguments.js",
                    "meta.function-call.method.without-arguments.js",
                    "source.scss",
                    "string source punctuation.section.embedded",
                    "punctuation.definition.tag.begin source",
                    "source.php"
                ],
                "settings": {
                    "foreground": "#99999C",                    
                }
            },
            {
                "scope": ["comment", "comment punctuation"],
                "settings": {
                    "foreground": "#88888B",                    
                }
            }
        ]
    },
    "window.commandCenter": false,
    "editor.fontLigatures": true,
    "editor.cursorSmoothCaretAnimation": "on",
    "editor.cursorBlinking": "smooth",
    "terminal.integrated.fontFamily": "JetBrains Mono NL",
    "terminal.integrated.fontLigatures.enabled": true,
    "terminal.integrated.lineHeight": 1.3,
    "terminal.integrated.scrollback": 10000,
    "terminal.integrated.cursorBlinking": true,
    "terminal.integrated.cursorStyle": "line",
    "terminal.integrated.cursorWidth": 2,    

    "files.exclude": {
        "**/.git": true,
        "**/.svn": true,
        "**/.hg": true,
        "**/.DS_Store": true,
        "**/Thumbs.db": true,
        "**/CVS": true,
        "node_modules": true,
    },

    "php.validate.executablePath": "/Applications/MAMP/bin/php/php8.3.28/bin/php",
}
```
