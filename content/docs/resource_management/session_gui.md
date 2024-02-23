---
title: Session Gui
type: docs
weight: 2
---

## Session gui prototype

The session gui consists on two vertically stacked panes containing multiple list views.

![Session Gui](images/sessiongui.jpg)
<p style="text-align: center;"><i>Figure 1: Prototype of the Session gui.</i></p>

The upper pane shows the bookmarks list and a file browser of two lists.  The file browser  for navigating the folders and files of the bookmarks list 

The lower pane shows a list of sessions, and the **configuration**, **server**, and **runtime** resources assigned to each session. 

## Workflow

1. Add folders or files that you want to use in your projects as bookmarks:
   - Click on the button "+ Bookmark" to create a new bookmark.
   - A file dialog opens.  Select a file or folder to make a new bookmark out of it.
   - The bookmark is named after the name of the file or folder selected.
   - To rename a bookmark, type "enter" on the selected bookmark item. 
2. Browse the contents of a selected bookmark 
   - If the bookmark is a folder, then the Outer List pane displays the name of the folder and the Inner List pane displays the name of the file selected.
   - The ```Text Field``` below the List panes shows the full path of the selected item. 
   - TODO: Add button shortcuts for navigating up and down the file tree from the Outer and Inner list panes.
   - TODO: Add button shortcut for adding the selected item as bookmark. 
   - Typing enter on a selected file, opens the file with a viewer depending on the file type:
     - If the file is an audio file (```.wav, .WAV, .aif, .AIF, .aiff, .AIFF```), then it opens with an audio file browser (part of ```sc-hacks-redux```). 
     - If the file is a time-tagged snippet file it opens with a score viewer (part of ```sc-hacks-redux```).
     - Else the file opens in the code editor of the current IDE (SuperCollider IDE or EMACS).
   - The outer list pane displays the name of the folder of 
3. Create a session by typing on the button ```+ Session```, or select an already existing session.
The ```Config``` ```Server``` and ```Runtime``` panes show any paths added to the corresponding category of the selected session.
Pressing any of the buttons ```+>Config```, ```+>Server``` or ```+>Runtime``` adds the selected path that is shown in the Text Field between the Bookmark pane and the Session pane. 
- TODO: Add mechanisms for deleting: paths from the resource categories, sessions, and bookmarks. 
- TODO: Add buttons for booting / quitting the server

## Useful Actions

Following actions should be made available by the interface:

### Bookmark Actions

- Create a bookmark:
  - Add as bookmark an item selected through a file dialog.
  - (Add as bookmark an item selected from the file browser pane - see below)
- Delete a bookmark
- Rename a bookmark

### File browser actions
  - Add as bookmark a file or folder selected on one of the list views of the content browser.
  - Add the selected item from one of the list views of the content browser to the *config*, *server* or *runtime* list. 

### Session Actions

- Create a session
- Delete a session
- Rename a session

### Session Item Actions
- Remove an item from the *config*, *server* or *runtime* list. 
- Open a browser on an item from the *config*, *server* or *runtime* list.

### Supplementary actions
- save the current bookmarks and session configurations
- load bookmarks and sessino configurations from a selected file.
- keep history of bookmark and session configurations (?)
- check all paths in bookmarks and sessions point to existing directories or files.
  - query user to provide alternatives or delete the entries for non-existing paths.

## Widgets to be added to the gui prototype: 


