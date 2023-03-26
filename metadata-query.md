---
date: 2023-03-26
type: idea
---

# Metadata query

Markdown has yaml frontmatter support, using either minus-metadata or
plus-metadata. This is also implemented in markdown lsp.

> minus-metadata
```markdown
---
tag: important
---
```

> plus-metadata
```markdown
+++
tag: important
+++
```

Idea is to enable users to query this data and return the corresponding markdown files.
For example, if I have a query like this:

```query
type=idea
```

This should list out the markdown files which have yaml frontmatter with type = idea

## Additional points

1. Let the user query the results from nvim-telescope
2. Let the user save the query and it gets auto-updated on save of the file
   (similar to what vimwiki does for dairy entries)

## Conclusion

This could be very powerful if we can query the frontmatter, a very powerful
tool to explore your notes.
