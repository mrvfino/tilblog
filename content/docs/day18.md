+++
title = 'Day 18: Firestore security rules are not filters'
date = 2024-02-01T23:11:46+08:00
draft = false
+++

I re-learned that queries for Firestore are as such. When it comes to creating rules for COLLECTION GROUP document queries you should use:

```
match {path=**}/foobars/{foobarId} {
    ...
}
```

instead of.

```
match /foobars/{foobarId} {
    ...
}
```

Took me almost half a day to remember and figure out.
