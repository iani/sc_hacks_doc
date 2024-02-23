---
title: Resources, Sessions, Bookmarks
type: docs
weight: 1
---

## Resources

A resource is a file that creates a data item. Examples of resources are: 

- An audio file
- An scd file containing SynthDef definitions. 
- An scd file containing score of timed code snippets and/or osc messages 
- An scd file that creates a Group or Collection of Groups
- An scd file that creates a Pattern or playable pattern template (```Pbind```, or in the case of sc-hacks, an ```EventStream```)
- An scd file that creates envelopes.
- An scd file that creates set of scales, tunings etc.
- A data set from motion capture, sound analysis or other sources.

Some kinds of resources may be required to load into memory when a certain condition is set.  There are three types of conditions: 

{{< callout emoji="✳️" >}}
1. **config resources**. These are loaded before booting the Server (e.g. to set some Server options.). Generally such resources are loaded at startup time (right after compiling the SuperCollider library).
2. **server resources** These are loaded when the Server is booted. (e.g. Sound Files, SynthDefs and Envelopes must be loaded to the Server after it has booted.) 
2. **runtime resources** These are loaded at a time decided by the user during the course of a piece or a work session (e.g. a score of actions or sensor messages).
{{< /callout >}}


## Sessions 

A session is a collection of resources used for a project such as a musical composition, a performance, an installation etc.  In a session, each resource is coupled with a tag marking when the resource should be loaded, i.e. (1.) at startup time or (2.) when the server is booted, or (3.) when asked by the server. 

## Bookmarks 

A bookmark is simply a path that is stored in order to be easily available for browsing. A collection of bookmarks thus makes it easy to browse the contents of folders located in different places on the user's system, and saves time from having to find them through the computer's system open file dialogue window.  The session gui provides a list view for browsing the list of bookmarks, for browsing the contents of the folder of a bookmark, and for adding paths from inside such a folder to a session. 
