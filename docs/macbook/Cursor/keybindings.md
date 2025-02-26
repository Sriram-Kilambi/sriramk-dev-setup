# Cursor Keybindings JSON

<code>
```
// Place your key bindings in this file to override the defaults
[
  {
    "key": "cmd+i cmd+e",
    "command": "aipopup.action.modal.generate",
    "when": "editorFocus && !composerBarIsVisible"
  },
  {
    "key": "cmd+k",
    "command": "-aipopup.action.modal.generate",
    "when": "editorFocus && !composerBarIsVisible"
  },
  {
    "key": "ctrl+shift+c ctrl+shift+o",
    "command": "workbench.panel.composerViewPane2"
  },
  {
    "key": "ctrl+shift+c ctrl+shift+h",
    "command": "workbench.panel.aichat"
  },
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
    "key": "ctrl+cmd+j",
    "command": "workbench.action.toggleMaximizedPanel"
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
    "key": "ctrl+w",
    "command": "workbench.action.closeActiveEditor"
  },
  {
    "key": "cmd+w",
    "command": "-workbench.action.closeActiveEditor"
  },
  {
    "key": "ctrl+t",
    "command": "workbench.action.gotoSymbol",
    "when": "!accessibilityHelpIsShown && !accessibleViewIsShown"
  },
  {
    "key": "shift+cmd+o",
    "command": "-workbench.action.gotoSymbol",
    "when": "!accessibilityHelpIsShown && !accessibleViewIsShown"
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
    "key": "ctrl+shift+alt+cmd+up",
    "command": "workbench.action.focusAboveGroup"
  },
  {
    "key": "cmd+r cmd+up",
    "command": "-workbench.action.focusAboveGroup"
  },
  {
    "key": "ctrl+shift+alt+cmd+down",
    "command": "workbench.action.focusBelowGroup"
  },
  {
    "key": "cmd+r cmd+down",
    "command": "-workbench.action.focusBelowGroup"
  },
  {
    "key": "ctrl+shift+alt+cmd+left",
    "command": "workbench.action.focusLeftGroup"
  },
  {
    "key": "cmd+r cmd+left",
    "command": "-workbench.action.focusLeftGroup"
  },
  {
    "key": "ctrl+shift+alt+cmd+right",
    "command": "workbench.action.focusRightGroup"
  },
  {
    "key": "cmd+r cmd+right",
    "command": "-workbench.action.focusRightGroup"
  },
  {
    "key": "alt+\\",
    "command": "workbench.action.splitEditorOrthogonal"
  },
  {
    "key": "cmd+r cmd+\\",
    "command": "-workbench.action.splitEditorOrthogonal"
  },
  {
    "key": "cmd+k u",
    "command": "workbench.action.closeUnmodifiedEditors"
  },
  {
    "key": "cmd+r u",
    "command": "-workbench.action.closeUnmodifiedEditors"
  },
  {
    "key": "cmd+k w",
    "command": "workbench.action.closeEditorsInGroup"
  },
  {
    "key": "cmd+r w",
    "command": "-workbench.action.closeEditorsInGroup"
  },
  {
    "key": "cmd+k z",
    "command": "workbench.action.toggleZenMode",
    "when": "!isAuxiliaryWindowFocusedContext"
  },
  {
    "key": "cmd+r z",
    "command": "-workbench.action.toggleZenMode",
    "when": "!isAuxiliaryWindowFocusedContext"
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
  },
  {
    "key": "shift+alt+cmd+p",
    "command": "workbench.action.pinEditor",
    "when": "!activeEditorIsPinned"
  },
  {
    "key": "cmd+r shift+enter",
    "command": "-workbench.action.pinEditor",
    "when": "!activeEditorIsPinned"
  },
  {
    "key": "shift+alt+cmd+p",
    "command": "workbench.action.unpinEditor",
    "when": "activeEditorIsPinned"
  },
  {
    "key": "cmd+r shift+enter",
    "command": "-workbench.action.unpinEditor",
    "when": "activeEditorIsPinned"
  },
  {
    "key": "ctrl+alt+cmd+[",
    "command": "editor.foldAll",
    "when": "editorTextFocus && foldingEnabled"
  },
  {
    "key": "cmd+r cmd+0",
    "command": "-editor.foldAll",
    "when": "editorTextFocus && foldingEnabled"
  },
  {
    "key": "ctrl+alt+cmd+]",
    "command": "editor.unfoldAll",
    "when": "editorTextFocus && foldingEnabled"
  },
  {
    "key": "cmd+r cmd+j",
    "command": "-editor.unfoldAll",
    "when": "editorTextFocus && foldingEnabled"
  },
  {
    "key": "ctrl+shift+d",
    "command": "editor.action.revealDefinition",
    "when": "editorHasDefinitionProvider && editorTextFocus"
  },
  {
    "key": "f12",
    "command": "-editor.action.revealDefinition",
    "when": "editorHasDefinitionProvider && editorTextFocus"
  },
  {
    "key": "shift+alt+cmd+m",
    "command": "workbench.action.toggleMaximizeEditorGroup",
    "when": "editorPartMaximizedEditorGroup || editorPartMultipleEditorGroups"
  },
  {
    "key": "cmd+r cmd+m",
    "command": "-workbench.action.toggleMaximizeEditorGroup",
    "when": "editorPartMaximizedEditorGroup || editorPartMultipleEditorGroups"
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
    "key": "cmd+c",
    "command": "editor.action.clipboardCopyAction"
  },
  {
    "key": "cmd+c",
    "command": "-editor.action.clipboardCopyAction"
  },
  {
    "key": "cmd+v",
    "command": "editor.action.clipboardPasteAction"
  },
  {
    "key": "cmd+v",
    "command": "-editor.action.clipboardPasteAction"
  }
]
```
</code>