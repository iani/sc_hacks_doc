---
title: Resource Implementation 
type: docs
weight: 3
---

Resources are stored in the Library.

Resource sets are stored as an archive in the User's SuperCollider folder for the given platform.

Points to discuss here: 

- Saving and reloading to/from file: When is the archive written? (at each change!)
- Keeping a history of older versions.
- Removing resources from the library
- Replacing resources when reloading. Checking if a resource with the same name already exists. Name resolution.
- Reloading resources at the right moment and order on server boot
- Loading and checking resource sets at startup
- Accessing resources by name (```\aSymbol```). 



