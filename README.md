# CrossReference

The aim of this repository is to collect the translations of referencing different objects inside the document, such as images, tables, listings, chapters, etc. 
The way in which items are cited inside the document changes from one language to another.

# Label and reference distinction

Labels are clearly different from references, for instance `Figure 1` could be referenced as `Figure 1` or `Fig. 1` depending on the context and the style used by the author.

## Labels

In most of the proffesional document editors, the labeling may be generated automatically. 
Hence the need of a stable and flexible standard for labeling different objects in the documents.

**Counter:** Counters are strings returned by de editor/compiler.
**Label type:** They indicate the type of object one is labeling in the document. 

This repository distinguishes between normal and abbreviated labels. 
Finally, for figures in english we would have two lines of yaml code
```
fugure-label: "Figure $(c)"
fugure-label-abbreviated: $Fig. $(c)"
```
where `$(c)` is an reference to the counter.
It should be up to the document editor one is using whether to add a separator so the final labeling end up being "Figure 2: " or "Fig. 2.-" deppending on the style.

