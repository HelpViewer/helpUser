# &#128214;Help Viewer quick guide

<!-- @print-keep-icons -->
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
    *(visible if defined by the help author or the indexing functionality is active)*

  These items are displayed as an expandable tree with clickable nodes. Clicking on an item expands its subcontent or opens the selected chapter.  
  &#x1F4C7; and &#x1F50E; have an input field at the top where you can search for an exact phrase.  
  Just start typing and press **Enter** to search.  
  Press **Esc** to clear the field.

  - &#x1F3E1; Go to the help file’s homepage (README.md)

### Viewer customization

  - 🌐 UI Language selection
  - 🕘 Search for other version (of help file) (Internet connection required)
  - &#127912; Switch color mode  
    *(color, greyscale, white to black, black to white, sepia)*
  - 📚 Show all chapters as book  
    *(after selecting page breaks and the method of printing Unicode icons in the text, simply click the button a second time and the result will be displayed)*  
    *(only chapters displayed in the topic tree, the help home page, and chapters referenced in the text are included in the output)*
  - ✏️ Notes  
*Allows you to add, manage, and toggle the display (👁️) or hiding (🙈) of user notes. Notes can be deleted by simply erasing their content. Those displayed on the screen are automatically included in the printout. They are only displayed when browsing individual chapters. Notes are stored only in your environment and no one else has access to them. However, if you switch to a different language or newer version of the same help file, your notes will also be displayed in it.*
  - &#8596; Move (toggle) sidebar to left/right
  - &#x1F532; Toggle UI to/from fullscreen
  - 📽 Presentation mode  
    *(full screen mode (🔲), keys ⬅, ⬆, ➡, ⬇ are used to switch between chapters/slides)*
  - 🌈 Select style  
    *(you can select a different application style from the drop-down list)*
  - &#x274C;&#xFE0E; Close left sidebar

## Right panel

The right panel displays the main content area:

- Current chapter/topic content
- Chapter title in the upper bar
- Action buttons:

  - &#x2630; Show left panel back  
    *(if hidden)*
  - 🖨️ Print current chapter
  - &#x2B05; Go to the previous chapter
  - &#x2B06; Go one level up
  - &#x27A1; Go to the next chapter
  - 📝 Edit in repository
  - 📥 Export the current chapter or all chapters
  
## Why something might be missing?

There are several reasons why certain elements may not appear:

| Missing icon or feature | Why? |
|---|---|
| &#x1F4D6; / &#x1F4C7; | These were not defined by the help file author |
| 🔎 | These were not defined by the help file author, the indexing function is disabled, or the indexing process has not been completed yet |
| &#x1F516; | The current chapter has no subchapters |
| &#x2630; | The left panel is already visible |
| Left panel | You closed the app with the panel hidden. Just click ☰ in the top bar to bring it back |
| 🕘 | Help is not linked to the public online repository or it is not accessible (e.g. no internet connection) |
| 📥 Export | The system administrator has removed the entire function or individual export formats from the application |

The 📥 Custom package feature allows you to customise most of the functionality. If it was used when downloading the application, some features may be unavailable.

## Configuration data

The application remembers your preferences using **local storage**:

| Key | Description |
|---|---|
| colorTheme | Selected color mode (&#127912;) |
| sidebarVisible | Visibility of the left panel (&#x274C;&#xFE0E; / &#x2630;) |
| language | Selected UI language (&#x1F310;) |
| keywordListingCount | Count of searched keywords in &#x1F4C7;, &#x1F50E; lists. |
| sidebarSide | Left panel side (&#8596; ; 0 = left, 1 = right) |
| printIcons | Unicode icons (characters) printing mode; 0 = remove, 1 = keep, 2 = author's configuration |
| notesVisible | User notes display mode; 0 = hidden (🙈), 1 = shown (👁️) |
| skin | Style/skin of application UI (🌈; empty = default) |
| exportDictionaries | For static export (if supported by the application): 1 = dictionaries will be exported (📇, 🔎), 0 = dictionaries will not be included in the export |

The ✏️ Notes module stores its data in the web browser's **IndexedDB** storage (database: **HelpViewer**).

# Getting started

## Opening help file

Append **?d={path}** to the viewer's URL to open a custom help file.
If omitted, the default file **hlp/Help-{selected language}.zip** will be loaded automatically.

The following are valid path formats that end with:

- .zip - zip help file
- / - directory on your disk or network URI address

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
| 🌐 Latest version download link | @LTOPVERSIONV@ |
