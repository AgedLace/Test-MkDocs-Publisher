---
title: Extended Markdown Syntax
slug: extended-syntax
date: 2024-08-11 09:32:57
update: 2024-08-12 09:00:48
publish: "true"
tags:
  - Formatting/Markdown/Extended-Syntax
categories: 
---
**SOURCE** - [Markdown Cheat Sheet | Markdown Guide](https://www.markdownguide.org/cheat-sheet/)

These elements extend the basic syntax by adding additional features. Not all Markdown applications support these elements.

### Table

```markdown
| Syntax    | Description |
| --------- | ----------- |
| Header    | Title       |
| Paragraph | Text        |
|           |             |
```

| Syntax    | Description |
| --------- | ----------- |
| Header    | Title       |
| Paragraph | Text        |
|           |             |

### Fenced Code Block

```
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

{  
  "firstName": "John",  
  "lastName": "Smith",  
  "age": 25  
}

### Footnote

```markdown
Here's a sentence with a footnote. [^1]

[^1]: This is the footnote.
```

### Heading ID

```markdown
### My Great Heading {#custom-id}
```

### Definition List

```markdown
term  
: definition
```

### Strikethrough

```markdown
~~The world is flat.~~
```

~~The world is flat.~~

### Task List

```markdown
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media
```

- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media

### Emoji

```markdown
That is so funny! :joy:
```

That is so funny! :joy:  
(See also [Copying and Pasting Emoji](https://www.markdownguide.org/extended-syntax/#copying-and-pasting-emoji))

### Highlight

```markdown
I need to highlight these ==very important words==.
```

I need to highlight these ==very important words==.

### Subscript

```markdown
H~2~O
```

H~2~O

### Superscript

```markdown
X^2^
```

X^2^
