---
title: ide-note
date: 2021-07-30 21:32:09
tags: ide, vscode
toc: true
---

# IDE features

## Multi-cursor editing

Using multiple cursors allows you to edit multiple parts of the document at once, greatly improving your productivity.

### Vscode

- Box Selection - ⇧↓, ⇧→, ⇧↑, ⇧← to select a block of text. ⇧⌥ while selecting text with the mouse or drag-select using the middle mouse button.
- Add a cursor - ⌥⌘↑ to add a new cursor above, or ⌥⌘↓ to add a new cursor below. You can also use your mouse with ⌥+Click to add a cursor anywhere.
- Create cursors on all occurrences of a string - select one instance of a string e.g. background-color and press ⇧⌘L. Now you can replace all instances by simply typing.

```css
#p1 {
  background-color: #ff0000;
} /* red in HEX format */
#p2 {
  background-color: hsl(120, 100%, 50%);
} /* green in HSL format */
#p3 {
  background-color: rgba(0, 4, 255, 0.733);
} /* blue with alpha channel in RGBA format */
```

## IntelliSense

### Vscode

- invoke IntelliSense: ⌃Space or ⌥Esc

```javascript
const canvas = document.querySelector('canvas');
const context = canvas.getContext('2d');

context.strokeStyle = 'blue';
context.
```

## Line Actions

### Vscode

- Copy a line and insert it above or below: ⇧⌥↓ or ⇧⌥↑
- Move an entire line or selection of lines up or down: ⌥↑ and ⌥↓
- Delete the entire line: ⇧⌘K.
- Comment out a line: ⌘/

```json
{
  "name": "John",
  "age": 31,
  "city": "New York"
}
```

## Refactoring

### Vscode

- Rename a function/variable: F2 or right-click on the function/variable name.

## Formatting

### Vscode

- Format a document: ⇧⌘F
- Format a selection: ⌘K ⌘F

ps: enable editor.formatOnSave

## Code Folding

### Vscode

- fold and unfold a block of code: ⌥⌘[ and ⌥⌘]
- fold and unfold all blocks: ⌘K ⌘0 and ⌘K ⌘J
- fold and unfold a number of levels: ⌘K ⌘1 to ⌘K ⌘5

## Errors and Warnings

### Vscode

- navigate to the next error: F8

## Code Snipets

### Vscode

- create a code snippet: Code > Preferences > User Snippets