---
Title: Markdown CheatSheet
Description: Introducing the installation process.
Author: Don Robertson
Robots: noindex,nofollow
Template: doc-item
---

This cheat sheet has been stolen from [The Markdown Guide](https://www.markdownguide.org)!

This Markdown cheat sheet provides a quick overview of all the Markdown syntax elements. It can’t cover every edge case, so if you need more information about any of these elements, refer to the reference guides for [basic syntax](https://www.markdownguide.org/basic-syntax) and [extended syntax](https://www.markdownguide.org/extended-syntax).

## Basic Syntax

These are the elements outlined in John Gruber’s original design document. All Markdown applications support these elements.

### Heading {#heading}

| Markdown | HTML |
| --- | --- |
| # H1 | `<h1>H1</h1>` |
| ## H2 | `<h2>H2</h2>` |
| ### H3 | `<h3>H3</h3>` |
| #### H4 | `<h4>H4</h4>` |
| ##### H5 | `<h5>H5</h5>` |
| ###### H6 | `<h6>H6</h6>` |

How they actually look.
# H1 Heading
## H2 Heading
### H3 Heading
#### H4 Heading
##### H5 Heading
###### H6 Heading

### Bold {#bold}
| Markdown | HTML |  |
| --- | --- | ---|
| `**bold text**` | `<strong>bold text</strong>`| **bold text**|

### Italic {#italic}
| Markdown | HTML |  |
| --- | --- | ---|
|`*italicized text*`|`<em>italicized text</em>`|*italicized text*|

### Blockquote {#blockquote}
| Markdown | HTML |
| --- | --- |
|`> Lorem ipsum dolor sit amet, consectetur adipiscing elit ... ` | `<blockquote><p>Lorem ipsum dolor sit amet, consectetur adipiscing elit ...</p> </blockquote>` |

> Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

```markdown
> Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. 
> 
> Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. 
```

> Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. 
> 
> Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. 


### Ordered List {#ordered_list}

```markdown 
1. First item 
2. Second item 
3. Third item 
```

```html
<ol>
  <li>First item </li>
  <li>Second item </li>
  <li>Third item </li>
</ol>
```

1. First item 
2. Second item 
3. Third item 


### Unordered List {#unordered_list}
```markdown
- First item
- Second item
- Third item
```
```html
<ul>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
</ul>
```
- First item
- Second item
- Third item

### Code {#code}

| Markdown | HTML |  |
| --- | --- | ---|
| <code>&#x60;code&#x60;</code>  | `<code>code</code>` | ``code`` |

### Horizontal Rule {#horizontal_rule}

| Markdown | HTML |
| --- | --- |
| `---` | `<hr>`|
---
### Link {#links}

| Markdown | HTML |  |
| --- | --- | ---|
|`[title](https://www.example.com)`|`<a href="https://www.example.com">title</a>`|[title](https://www.example.com)|

### Image {#image}

| Markdown | HTML | 
| --- | --- | 
|`![alt text](/docs/images/moon.jpg)`| `<img src="/docs/images/moon.jpg" alt="alt text">` |

![alt text](/docs/images/moon.jpg)


## Extended Syntax {#extended_syntax}

These elements extend the basic syntax by adding additional features. Not all Markdown applications support these elements.

### Table {#table}
```markdown
| Syntax | Description |
| ----------- | ----------- |
| Header | Title |
| Paragraph | Text |
```
| Syntax | Description |
| ----------- | ----------- |
| Header | Title |
| Paragraph | Text |

### Fenced Code Block {#code_block}

<pre>
<code>
&#x60;&#x60;&#x60;
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
&#x60;&#x60;&#x60;
</code>
</pre>
```
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

### Footnote {#footnote}

| Markdown | HTML |  |
| --- | --- | ---|
| `Here's a sentence with a footnote. [^1]`||Here's a sentence with a footnote. [^1]|

`[^1]: This is the footnote.`
The footnote is at the bottom.
[^1]: This is the footnote.

### Heading ID

| Markdown | HTML |
| --- | --- | 
| `### My Great Heading {#custom-id}`|`<h3 id="custom-id">My Great Heading</h3>`|
### My Great Heading {#custom-id}

### Definition List {#definition_list}
```
term
: definition
```

term
: definition

### Strikethrough {#strikethrough}

| Markdown | HTML | |
| --- | --- | --- |
| `~~The world is flat.~~`|`<del>The world is flat.</del>`|~~The world is flat.~~|

### Task List {#tasklist}
```
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media
```
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media
