---
title: Obsidian-Basic-Formatting
slug: obsidian-basic
date: 2024-08-11 10:44:54
update: 2024-08-12 05:47:18
publish: "true"
tags:
  - Formatting/Markdown/Obsidian/Basic
categories: 
---
**SOURCE** - [Basic formatting syntax - Obsidian Help](https://help.obsidian.md/Editing+and+formatting/Basic+formatting+syntax)

Learn how to apply basic formatting to your notes, using [Markdown](https://daringfireball.net/projects/markdown/). For more advanced formatting syntax, refer to [[Obsidian-Advanced-Formatting]].

## Paragraphs

To create paragraphs, use a blank line to separate one or more lines of text.

```markdown
This is a paragraph.

This is another paragraph.
```

> [!note]- Multiple blank spaces  
> Multiple adjacent blank spaces in and between paragraphs collapse to a single space when displaying a note in Reading view and on Obsidian Publish sites.
> 
> ```md
> Multiple          adjacent          spaces
> 
> 
> 
> and multiple newlines between paragraphs.
> ```
> > 
> > Multiple adjacent spaces
> > 
> > 
> > 
> > and multiple newlines between paragraphs.
> 
> If you want to add multiple spaces, you can add `&nbsp;` (blank space) and `<br>` (newline) to your note.

## Headings

To create a heading, add up to six `#` symbols before your heading text. The number of `#` symbols determines the size of the heading.

```md
# This is a heading 1
## This is a heading 2
### This is a heading 3
#### This is a heading 4
##### This is a heading 5
###### This is a heading 6
```

%% These headings use HTML to avoid cluttering the Outline/Table of contents %%

<h1>This is a heading 1</h1>
<h2>This is a heading 2</h2>
<h3>This is a heading 3</h3>
<h4>This is a heading 4</h4>
<h5>This is a heading 5</h5>
<h6>This is a heading 6</h6>

## Bold, Italics, Highlights

Text formatting can also be applied using Editing shortcuts.

| Style | Syntax | Example | Output |
|-|-|-|-|
| Bold | `** **` or `__ __` | `**Bold text**` | **Bold text** |
| Italic | `* *` or `_ _`  | `*Italic text*` | *Italic text* |
| Strikethrough | `~~ ~~` |  `~~Striked out text~~` | ~~Striked out text~~ |
| Highlight | `== ==` |  `==Highlighted text==` | ==Highlighted text== |
| Bold and nested italic | `** **` and `_ _`  | `**Bold text and _nested italic_ text**` | **Bold text and *nested italic* text** |
| Bold and italic | `*** ***` or `___ ___` |  `***Bold and italic text***` | ***Bold and italic text*** |

Formatting can be forced to display in plain text by adding a backslash `\` in front of it.

\*\*This line will not be bold\*\*

```markdown
\*\*This line will not be bold\*\*
```

\**This line will be italic and show the asterisks*\*

```markdown
\**This line will be italic and show the asterisks*\*
```

## Internal Links

Obsidian supports two formats for internal links between notes:

- Wikilink: `[[Three laws of motion]]`
- Markdown: `[Three laws of motion](Three%20laws%20of%20motion.md)`

## External Links

If you want to link to an external URL, you can create an inline link by surrounding the link text in brackets (`[ ]`), and then the URL in parentheses (`( )`).

```md
[Obsidian Help](https://help.obsidian.md)
```

[Obsidian Help](https://help.obsidian.md)

You can also create external links to files in other vaults, by linking to an Obsidian URI.

```md
[Note](obsidian://open?vault=MainVault&file=Note.md)
```

### Escape Blank Spaces in Links

If your URL contains blank spaces, you must escape them by replacing them with `%20`.

```md
[My Note](obsidian://open?vault=MainVault&file=My%20Note.md)
```

You can also escape the URL by wrapping it with angled brackets (`< >`).

```md
[My Note](<obsidian://open?vault=MainVault&file=My Note.md>)
```

## External Images

You can add images with external URLs, by adding a `!` symbol before an external link.

```md
![Engelbart](https://history-computer.com/ModernComputer/Basis/images/Engelbart.jpg)
```

![Engelbart](https://history-computer.com/ModernComputer/Basis/images/Engelbart.jpg)

You can change the image dimensions, by adding `|640x480` to the link destination, where 640 is the width and 480 is the height.

```md
![Engelbart|100x145](https://history-computer.com/ModernComputer/Basis/images/Engelbart.jpg)
```

If you only specify the width, the image scales according to its original aspect ratio. For example:

```md
![Engelbart|100](https://history-computer.com/ModernComputer/Basis/images/Engelbart.jpg)
```

> [!tip]  
> If you want to add an image from inside your vault, you can also embed an image in a note.

## Quotes

You can quote text by adding a `>` symbols before the text.

```md
> Human beings face ever more complex and urgent problems, and their effectiveness in dealing with these problems is a matter that is critical to the stability and continued progress of society.

\- Doug Engelbart, 1961
```

> Human beings face ever more complex and urgent problems, and their effectiveness in dealing with these problems is a matter that is critical to the stability and continued progress of society.

\- Doug Engelbart, 1961

> [!tip]  
> You can turn your quote into a callout by adding `[!info]` as the first line in a quote.

## Lists

You can create an unordered list by adding a `-`, `*`, or `+` before the text.

```md
- First list item
- Second list item
- Third list item
```

- First list item
- Second list item
- Third list item

To create an ordered list, start each line with a number followed by a `.` symbol.

```md
1. First list item
2. Second list item
3. Third list item
```

1. First list item
2. Second list item
3. Third list item

### Task Lists

To create a task list, start each list item with a hyphen and space followed by `[ ]`.

```md
- [x] This is a completed task.
- [ ] This is an incomplete task.
```

- [x] This is a completed task.
- [ ] This is an incomplete task.

You can toggle a task in Reading view by selecting the checkbox.

> [!tip]  
> You can use any character inside the brackets to mark it as complete.
> 
> ```md
> - [x] Milk
> - [?] Eggs
> - [-] Eggs
> ```
> 
> - [x] Milk
> - [?] Eggs
> - [-] Eggs

### Nesting Lists

All list types can be nested in Obsidian.

To create a nested list, indent one or more list items:

```md
1. First list item
   1. Ordered nested list item
2. Second list item
   - Unordered nested list item
```

1. First list item
   1. Ordered nested list item
2. Second list item
   - Unordered nested list item

Similarly, you can create a nested task list by indenting one or more list items:

```md
- [ ] Task item 1
	- [ ] Subtask 1
- [ ] Task item 2
	- [ ] Subtask 1
```

- [ ] Task item 1
	- [ ] Subtask 1
- [ ] Task item 2
	- [ ] Subtask 1

Use `Tab` or `Shift+Tab` to indent or unindent one or more selected list items for easy organization.

## Horizontal Rule

You can use three or more stars `***`, hyphens `---`, or underscore `___` on its own line to add a horizontal bar. You can also separate symbols using spaces.

```md
***
****
* * *
---
----
- - -
___
____
_ _ _
```

***

## Code

You can format code both inline within a sentence, or in its own block.

### Inline Code

You can format code within a sentence using single backticks.

```md
Text inside `backticks` on a line will be formatted like code.
```

Text inside `backticks` on a line will be formatted like code.

If you want to put backticks in an inline code block, surround it with double backticks like so: inline ``code with a backtick ` inside``.

### Code Blocks

To format a block of code, surround the code with triple backticks.

~~~
```
cd ~/Desktop
```
~~~

```md
cd ~/Desktop
```

You can also create a code block by indenting the text using `Tab` or 4 blank spaces.

```md
    cd ~/Desktop
```

You can add syntax highlighting to a code block, by adding a language code after the first set of backticks.

~~~md
```js
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }
}
```
~~~

```js
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }
}
```

Obsidian uses Prism for syntax highlighting. For more information, refer to [Supported languages](https://prismjs.com/#supported-languages).

> [!note]  
> Source mode and Live Preview do not support PrismJS, and may render syntax highlighting differently.

## Footnotes

You can add footnotes[^1] to your notes using the following syntax:

```md
This is a simple footnote[^1].

[^1]: This is the referenced text.
[^2]: Add 2 spaces at the start of each new line.
  This lets you write footnotes that span multiple lines.
[^note]: Named footnotes still appear as numbers, but can make it easier to identify and link references.
```

You can also inline footnotes in a sentence. Note that the caret goes outside the brackets.

```md
You can also use inline footnotes. ^[This is an inline footnote.]
```

> [!note]  
> Inline footnotes only work in reading view, not in Live Preview.

## Comments

You can add comments by wrapping text with `%%`. Comments are only visible in Editing view.

```md
This is an %%inline%% comment.

%%
This is a block comment.

Block comments can span multiple lines.
%%
```

[^1]: This is a footnote.
