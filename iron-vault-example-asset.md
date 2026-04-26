Markdown asset files
To make it easier to create Assets, Iron Vault supports a straightforward Markdown format for creating Assets. Here's an example Asset Markdown file:

```
---
type: asset
---

# Asset name (Asset path)

Once you write an asset... (this optional paragraph becomes the "requirement")

## Abilities

* [x] This is a default checked ability.
* [ ] This is a default unchecked ability.
* [ ] Right now abilities aren't parsed for anything (so, e.g., you can't currently embed custom asset moves)

## Controls

* health (condition meter, max: 3)
  * weakened (checkbox, is_impact: true)

## Options

* pen name (text)
```

Frontmatter:

The type frontmatter property must say asset. That's how Iron Vault knows you want this to be parsed as an Asset file.
All other frontmatter properties will be added to the Datasworn Source Asset object as-is.
The Abilities section is mandatory; however you may omit the ## Abililties header if you'd like.

The Controls and Options sections are optional and can appear in any order, as long as they are after the mandatory Abilities section.