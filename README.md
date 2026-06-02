### Security

- parser: Pass userData to SAX text callbacks in xmlParseReference (type-confusion)
- entities: copy children in xmlCopyEntity
- c14n: Fix Type confusion in xmlC14NProcessAttrsAxis
- python: Do not decref string after adding to the list (double-free / use-after-free)
- c14n: Reuse tmp_str, xmlStrcat reallocates *cur (double-free)

### Improvements

- schemas: Fix relative schemaLocation resolution in XSI assembly in streaming mode
- xmlreader: propagate reader resource loaders to validator parsers
- python: Make python bindings python2 compatible
- xmlregexp: Fix escape-sequence character range matching
- xmlreader: Free input in xmlReaderForFd (memory-leak)
- xmlstring: Free cur on every error for xmlStrncat (memory-leak)
- catalog: Free xmlCatalogResolveCache on cleanup (memory leak)
- Fix nanohttp.c build when --without-output
- test: fix mismatched signed/unsigned comparison

### Thanks

Thanks to the following new contributors:

- Ariel Schon
- Hieu Le Minh
- James Lan
- LCaliman
- Yenya

### Full list of commits and contributors on this release

13  Daniel Garcia Moreno
 2  Ariel Schon
 2  Hieu Le Minh
 1  James Lan
 1  Jan Alexander Steffens (heftig)
 1  LCaliman
 1  Yenya
