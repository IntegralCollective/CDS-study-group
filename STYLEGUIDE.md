# Style guide

**Note:** this is a work-in-progress.

## Semantic Line Breaks

We're aiming to use Semantic Line Breaks, which describe a set of conventions for using insensitive vertical whitespace to structure prose along semantic boundaries.

## Glossary

A term in the glossary should never be used to mean anything other than its meaning in the glossary. And if you're talking about something defined in the glossary, you should never use other words to describe it than the one in the glossary.

The first time a term from the glossary is mentioned on a page, it should link to the definition in the glossary. For example, from the `docs` folder, you can use a relative path:

```markdown
[participant](../glossary.md#participant)
```

In the future we can try to automate this, so that we don't have to remember it, but, for now, try to keep it in mind.
