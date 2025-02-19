# VS Code Keybindings JSON

<code>
```
// Place your key bindings in this file to override the defaultsauto[]
[
  {
    "key": "ctrl+shift+up",
    "command": "editor.action.insertCursorAbove",
    "when": "editorTextFocus"
  },
  {
    "key": "alt+cmd+up",
    "command": "-editor.action.insertCursorAbove",
    "when": "editorTextFocus"
  },
  {
    "key": "ctrl+shift+down",
    "command": "editor.action.insertCursorBelow",
    "when": "editorTextFocus"
  },
  {
    "key": "alt+cmd+down",
    "command": "-editor.action.insertCursorBelow",
    "when": "editorTextFocus"
  },
  {
    "key": "shift+alt+q",
    "command": "editor.action.toggleMinimap"
  },
  {
    "key": "ctrl+shift+alt+f",
    "command": "editor.action.formatDocument",
    "when": "editorHasDocumentFormattingProvider && editorTextFocus && !editorReadonly && !inCompositeEditor"
  },
  {
    "key": "shift+alt+f",
    "command": "-editor.action.formatDocument",
    "when": "editorHasDocumentFormattingProvider && editorTextFocus && !editorReadonly && !inCompositeEditor"
  },
  {
    "key": "ctrl+shift+alt+f",
    "command": "editor.action.formatDocument.none",
    "when": "editorTextFocus && !editorHasDocumentFormattingProvider && !editorReadonly"
  },
  {
    "key": "shift+alt+f",
    "command": "-editor.action.formatDocument.none",
    "when": "editorTextFocus && !editorHasDocumentFormattingProvider && !editorReadonly"
  },
  {
    "key": "ctrl+tab",
    "command": "workbench.action.nextEditor"
  },
  {
    "key": "shift+cmd+]",
    "command": "-workbench.action.nextEditor"
  },
  {
    "key": "ctrl+shift+tab",
    "command": "workbench.action.previousEditor"
  },
  {
    "key": "shift+cmd+[",
    "command": "-workbench.action.previousEditor"
  },
  {
    "key": "ctrl+shift+alt+cmd+left",
    "command": "workbench.action.focusLeftGroup"
  },
  {
    "key": "cmd+k cmd+left",
    "command": "-workbench.action.focusLeftGroup"
  },
  {
    "key": "ctrl+shift+alt+cmd+right",
    "command": "workbench.action.focusRightGroup"
  },
  {
    "key": "cmd+k cmd+right",
    "command": "-workbench.action.focusRightGroup"
  },
  {
    "key": "ctrl+shift+d",
    "command": "editor.action.revealDefinition",
    "when": "editorHasDefinitionProvider && editorTextFocus && !isInEmbeddedEditor"
  },
  {
    "key": "f12",
    "command": "-editor.action.revealDefinition",
    "when": "editorHasDefinitionProvider && editorTextFocus && !isInEmbeddedEditor"
  },
  {
    "key": "ctrl+w",
    "command": "workbench.action.closeActiveEditor"
  },
  {
    "key": "cmd+w",
    "command": "-workbench.action.closeActiveEditor"
  },
  {
    "key": "ctrl+w",
    "command": "workbench.action.closeWindow",
    "when": "!editorIsOpen && !multipleEditorGroups"
  },
  {
    "key": "cmd+w",
    "command": "-workbench.action.closeWindow",
    "when": "!editorIsOpen && !multipleEditorGroups"
  },
  {
    "key": "ctrl+w",
    "command": "workbench.action.terminal.killEditor",
    "when": "terminalEditorFocus && terminalFocus && terminalHasBeenCreated && resourceScheme == 'vscode-terminal' || terminalEditorFocus && terminalFocus && terminalProcessSupported && resourceScheme == 'vscode-terminal'"
  },
  {
    "key": "cmd+w",
    "command": "-workbench.action.terminal.killEditor",
    "when": "terminalEditorFocus && terminalFocus && terminalHasBeenCreated && resourceScheme == 'vscode-terminal' || terminalEditorFocus && terminalFocus && terminalProcessSupported && resourceScheme == 'vscode-terminal'"
  },
  {
    "key": "ctrl+w",
    "command": "workbench.action.closeGroup",
    "when": "activeEditorGroupEmpty && multipleEditorGroups"
  },
  {
    "key": "cmd+w",
    "command": "-workbench.action.closeGroup",
    "when": "activeEditorGroupEmpty && multipleEditorGroups"
  },
  {
    "key": "cmd+w",
    "command": "workbench.action.switchWindow"
  },
  {
    "key": "ctrl+w",
    "command": "-workbench.action.switchWindow"
  },
  {
    "key": "shift+cmd+o",
    "command": "editor.action.transposeLetters",
    "when": "textInputFocus && !editorReadonly"
  },
  {
    "key": "ctrl+t",
    "command": "-editor.action.transposeLetters",
    "when": "textInputFocus && !editorReadonly"
  },
  {
    "key": "ctrl+t",
    "command": "workbench.action.gotoSymbol"
  },
  {
    "key": "shift+cmd+o",
    "command": "-workbench.action.gotoSymbol"
  },
  {
    "key": "ctrl+cmd+j",
    "command": "workbench.action.toggleMaximizedPanel"
  },
  {
    "key": "alt+\\",
    "command": "workbench.action.splitEditorOrthogonal"
  },
  {
    "key": "cmd+k cmd+\\",
    "command": "-workbench.action.splitEditorOrthogonal"
  },
  {
    "key": "ctrl+shift+alt+cmd+up",
    "command": "workbench.action.focusAboveGroup"
  },
  {
    "key": "cmd+k cmd+up",
    "command": "-workbench.action.focusAboveGroup"
  },
  {
    "key": "ctrl+shift+alt+cmd+down",
    "command": "workbench.action.focusBelowGroup"
  },
  {
    "key": "cmd+k cmd+down",
    "command": "-workbench.action.focusBelowGroup"
  },
  {
    "key": "alt+cmd+h",
    "command": "editor.action.startFindReplaceAction",
    "when": "editorFocus || editorIsOpen"
  },
  {
    "key": "alt+cmd+f",
    "command": "-editor.action.startFindReplaceAction",
    "when": "editorFocus || editorIsOpen"
  },
  {
    "key": "ctrl+shift+cmd+c",
    "command": "git.checkout"
  },
  {
    "key": "shift+alt+cmd+p",
    "command": "workbench.action.pinEditor",
    "when": "!activeEditorIsPinned"
  },
  {
    "key": "cmd+k shift+enter",
    "command": "-workbench.action.pinEditor",
    "when": "!activeEditorIsPinned"
  },
  {
    "key": "shift+alt+cmd+p",
    "command": "workbench.action.unpinEditor",
    "when": "activeEditorIsPinned"
  },
  {
    "key": "cmd+k shift+enter",
    "command": "-workbench.action.unpinEditor",
    "when": "activeEditorIsPinned"
  },
  {
    "key": "ctrl+alt+cmd+[",
    "command": "editor.foldAll",
    "when": "editorTextFocus && foldingEnabled"
  },
  {
    "key": "cmd+k cmd+0",
    "command": "-editor.foldAll",
    "when": "editorTextFocus && foldingEnabled"
  },
  {
    "key": "ctrl+alt+cmd+]",
    "command": "editor.unfoldAll",
    "when": "editorTextFocus && foldingEnabled"
  },
  {
    "key": "cmd+k cmd+j",
    "command": "-editor.unfoldAll",
    "when": "editorTextFocus && foldingEnabled"
  },
  {
    "key": "ctrl+shift+alt+cmd+m",
    "command": "workbench.action.toggleMaximizeEditorGroup",
    "when": "maximizedEditorGroup || multipleEditorGroups"
  },
  {
    "key": "cmd+k cmd+m",
    "command": "-workbench.action.toggleMaximizeEditorGroup",
    "when": "maximizedEditorGroup || multipleEditorGroups"
  },
  {
    "key": "ctrl+shift+alt+p ctrl+shift+alt+i",
    "command": "workbench.panel.chat.view.copilot.focus"
  },
  {
    "key": "ctrl+shift+alt+;",
    "command": "github.copilot.interactiveEditor.explain"
  },
  {
    "key": "alt+cmd+z",
    "command": "editor.action.toggleWordWrap"
  },
  {
    "key": "alt+z",
    "command": "-editor.action.toggleWordWrap"
  },
  {
    "key": "shift+alt+cmd+b",
    "command": "bookmarks.toggle",
    "when": "editorTextFocus"
  },
  {
    "key": "alt+cmd+k",
    "command": "-bookmarks.toggle",
    "when": "editorTextFocus"
  },
  {
    "key": "shift+alt+cmd+,",
    "command": "bookmarks.jumpToPrevious",
    "when": "editorTextFocus"
  },
  {
    "key": "alt+cmd+j",
    "command": "-bookmarks.jumpToPrevious",
    "when": "editorTextFocus"
  },
  {
    "key": "shift+alt+cmd+.",
    "command": "bookmarks.jumpToNext",
    "when": "editorTextFocus"
  },
  {
    "key": "alt+cmd+l",
    "command": "-bookmarks.jumpToNext",
    "when": "editorTextFocus"
  }
]
```
</code>