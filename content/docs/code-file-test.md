---
title: Code Snippet Test 
type: docs
prev: /
<!-- next: docs/folder/ -->
weight: 10000
---

Testing how inline code is displayed.
The code fragment below should have the file "main.sc" in the header, followed by some token contents in the sc language.
The type given is js because I do not have a coloring template for js yet.

## Hello, World!

```js {filename="main.sc"}
{ [1, 0].choose.postln; } ! 10;
{
    WhiteNoise.ar(0.1).dup
} +> \testing;
```
