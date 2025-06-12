# &#128214;Help Viewer quick guide

The application is divided into two main areas:

## Left panel

The left panel lets you navigate through the help file.

At the bottom of this panel, you’ll find several buttons:

### Help navigation

  - &#x1F4D6; Hierarchical TOC (Table of Contents) tree  
    *(visible if defined by the help author)*
  - &#x1F516; Subchapter list  
    *(shown if the current chapter has subchapters)*
  - &#x1F4C7; Keywords list / Glossary  
    *(visible if defined by the help author)*
  - &#x1F50E; Fulltext keywords list  
    *(visible if defined by the help author)*

  These items are displayed as an expandable tree with clickable nodes. Clicking on an item expands its subcontent or opens the selected chapter.  
  &#x1F4C7; and &#x1F50E; have an input field at the top where you can search for an exact phrase.  
  Just start typing and press **Enter** to search.  
  Press **Esc** to clear the field.

  - &#x1F3E1; Go to the help file’s homepage (README.md)

### Viewer customization

  - &#x1F310; UI Language selection
  - &#127912; Switch color mode  
    *(color, greyscale, white to black, black to white)*
  - &#x1F532; Toggle UI to/from fullscreen
  - &#x274C;&#xFE0E; Close left sidebar

## Right panel

The right panel displays the main content area:

- Current chapter/topic content
- Chapter title in the upper bar
- Action buttons:

  - &#x2630; Show left panel back  
    *(if hidden)*
  - &#x1F4C4; Print current chapter
  - &#x2B05; Go to the previous chapter
  - &#x2B06; Go one level up
  - &#x27A1; Go to the next chapter
  
## Why something might be missing?

There are several reasons why certain elements may not appear:

| Missing icon or feature | Why? |
|---|---|
| &#x1F4D6; / &#x1F4C7; | These were not defined by the help file author |
| &#x1F516; | The current chapter has no subchapters |
| &#x2630; | The left panel is already visible |
| Left panel | You closed the app with the panel hidden. Just click ☰ in the top bar to bring it back |

## Session Data

The application remembers your preferences using **local storage**:

| Key | Description |
|---|---|
| colorTheme | Selected color mode (&#127912;) |
| sidebarVisible | Visibility of the left panel (&#x274C;&#xFE0E; / &#x2630;) |
| language | Selected UI language (&#x1F310;) |
| keywordListingCount | Count of searched keywords in &#x1F4C7;, &#x1F50E; lists. |

# Getting started

## Opening help file

Append **?d={path}** to the viewer's URL to open a custom help file.
If omitted, the default file **hlp/Help-{selected language}.zip** will be loaded automatically.

## Browser tips

Modern web browsers include built-in features such as:

### 🧭 Content Navigation

| Shortcut | Action |
|---|---|
| Tab | Go to next button / link on the page |
| SHIFT + Tab | Go to previous button / link on the page |
| ↑ ↓ ← → | Scroll or move focus inside content (if possible) |
| PageUp / PageDown | Jump one page up/down in content |

### &#127760; Browser Navigation & Page Actions

| Shortcut | Action |
|---|---|
| ALT + ← / → | Navigate back/forward in history |
| CTRL + L | Focus address bar |
| CTRL + D | Bookmark current page |

### &#x1F50D; Display & magnification

| Shortcut | Action |
|---|---|
| CTRL + mouse wheel | Zoom in / Zoom out |
| CTRL + 0 | Reset zoom |
| F11 | Toggle / Exit fullscreen mode (page or iframe) |
| ESC | Exit fullscreen mode |
| F3 / CTRL + F | Find text on page |

### &#x1F501; Content reload

| Shortcut | Action |
|---|---|
| CTRL + R / F5 | Reload page |
| CTRL + SHIFT + R | Hard reload (bypass cache) |

### &#x1F4BE; Application & Install

| Shortcut | Action |
|---|---|
| Address bar icon (&#x1F4E5;) on right side | Install web app |
