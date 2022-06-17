---
title: cache
version: 0.64.0
usage: |
  Caches operations in a new LazyFrame
---

<script>
  import { usePageFrontmatter } from '@vuepress/client';
  export default { computed: { frontmatter() { return usePageFrontmatter().value; } } }
</script>

# <code>{{ frontmatter.title }}</code>

<div style='white-space: pre-wrap;'>{{ frontmatter.usage }}</div>

## Signature

```> cache ```

## Examples

Caches the result into a new LazyFrame
```shell
> [[a b]; [6 2] [4 2] [2 2]] | to-df | reverse | cache
```