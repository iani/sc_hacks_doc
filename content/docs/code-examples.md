---
title: Code Examples 
type: docs
weight: 10
<!-- prev: / -->
<!-- next: docs/folder/ -->
<!-- weight: 10000 -->
---

Here are some examples of making sound with sc-hacks:

## Play a sound function

```js {filename="functin_play.sc"}
{ WhiteNoise.ar(0.1).dup } +> \test;
```

## Play an event as a pattern

```js {filename="functin_play.sc"}
{ WhiteNoise.ar(0.1).dup } +> \test;
```

Note that the event pattern replaces the synth previously started by the function.
