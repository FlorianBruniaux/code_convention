# Code and Syntax Highlighting

Example:

    ```javascript
    var s = "JavaScript syntax highlighting";
    alert(s);
    ```
```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```
    
    ```php
    $path = "";
	$rubrique = "contact";
	$title="Véhicules E-motors";
	include("includes/db_connect.php");
	include("includes/functions.php");
    ```
```php
$path = "";
$rubrique = "contact";
$title="Véhicules E-motors";
include("includes/db_connect.php");
include("includes/functions.php");
```

    ```
    No language indicated, so no syntax highlighting.
    s = "There is no highlighting for this."
    But let's throw in a <b>tag</b>.
    ```

```
No language indicated, so no syntax highlighting.
s = "There is no highlighting for this."
But let's throw in a <b>tag</b>.
```

- @foo : for team members
- @all : for the whole team
- #123 : for issues
- !123 : for merge requests
- $123 : for snippets
- 1234567 : for commits
- \[file\](path/to/file) : for file references

GFM also recognizes references to commits, issues, and merge requests in other projects:

- namespace/project#123 : for issues
- namespace/project!123 : for merge requests
- namespace/project@1234567 : for commits

## Task Lists

You can add task lists to merge request and issue descriptions to keep track of to-do items.  To create a task, add an unordered list to the description in an issue or merge request, formatted like so:

```no-highlight
* [x] Completed task
* [ ] Unfinished task
    * [x] Nested task
```

Task lists can only be created in descriptions, not in titles or comments.  Task item state can be managed by editing the description's Markdown or by clicking the rendered checkboxes.

# Standard Markdown

## Headers

```no-highlight
# H1
## H2
### H3
#### H4
##### H5
###### H6


## Emphasis

```no-highlight
Emphasis, aka italics, with *asterisks* or _underscores_.

Strong emphasis, aka bold, with **asterisks** or __underscores__.

Combined emphasis with **asterisks and _underscores_**.

Strikethrough uses two tildes. ~~Scratch this.~~
```

Emphasis, aka italics, with *asterisks* or _underscores_.

Strong emphasis, aka bold, with **asterisks** or __underscores__.

Combined emphasis with **asterisks and _underscores_**.

Strikethrough uses two tildes. ~~Scratch this.~~

## Lists

```no-highlight
1. First ordered list item
2. Another item
  * Unordered sub-list.
1. Actual numbers don't matter, just that it's a number
  1. Ordered sub-list
4. And another item.

   Some text that should be aligned with the above item.

* Unordered list can use asterisks
- Or minuses
+ Or pluses
```

1. First ordered list item
2. Another item
  * Unordered sub-list.
1. Actual numbers don't matter, just that it's a number
  1. Ordered sub-list
4. And another item.

   Some text that should be aligned with the above item.

* Unordered list can use asterisks
- Or minuses
+ Or pluses

## Links

There are two ways to create links, inline-style and reference-style.

    [I'm an inline-style link](https://www.google.com)

    [I'm a reference-style link][Arbitrary case-insensitive reference text]

    [I'm a relative reference to a repository file](LICENSE)

    [You can use numbers for reference-style link definitions][1]

    Or leave it empty and use the [link text itself][]

    Some text to show that the reference links can follow later.

    [arbitrary case-insensitive reference text]: https://www.mozilla.org
    [1]: http://slashdot.org
    [link text itself]: http://www.reddit.com

[I'm an inline-style link](https://www.google.com)

[I'm a reference-style link][Arbitrary case-insensitive reference text]

[I'm a relative reference to a repository file](LICENSE)

[You can use numbers for reference-style link definitions][1]

Or leave it empty and use the [link text itself][]

Some text to show that the reference links can follow later.

[arbitrary case-insensitive reference text]: https://www.mozilla.org
[1]: http://slashdot.org
[link text itself]: http://www.reddit.com

**Note**

Relative links do not allow referencing project files in a wiki page or wiki page in a project file. The reason for this is that, in GitLab, wiki is always a separate git repository. For example:

`[I'm a reference-style link][style]`

will point the link to `wikis/style` when the link is inside of a wiki markdown file.

## Images

    Here's our logo (hover to see the title text):

    Inline-style:
    ![alt text](assets/logo-white.png)

    Reference-style:
    ![alt text1][logo]

    [logo]: assets/logo-white.png

Here's our logo:

Inline-style:

![alt text](/assets/logo-white.png)

Reference-style:

![alt text][logo]

[logo]: /assets/logo-white.png

## Blockquotes

```no-highlight
> Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.

Quote break.

> This is a very long line that will still be quoted properly when it wraps. Oh boy let's keep writing to make sure this is long enough to actually wrap for everyone. Oh, you can *put* **Markdown** into a blockquote.
```

> Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.

Quote break.

> This is a very long line that will still be quoted properly when it wraps. Oh boy let's keep writing to make sure this is long enough to actually wrap for everyone. Oh, you can *put* **Markdown** into a blockquote.

## Inline HTML

You can also use raw HTML in your Markdown, and it'll mostly work pretty well.

```no-highlight
<dl>
  <dt>Definition list</dt>
  <dd>Is something people use sometimes.</dd>

  <dt>Markdown in HTML</dt>
  <dd>Does *not* work **very** well. Use HTML <em>tags</em>.</dd>
</dl>
```

<dl>
  <dt>Definition list</dt>
  <dd>Is something people use sometimes.</dd>

  <dt>Markdown in HTML</dt>
  <dd>Does *not* work **very** well. Use HTML <em>tags</em>.</dd>
</dl>


## Tables


```
| header 1 | header 2 |
| -------- | -------- |
| cell 1   | cell 2   |
| cell 3   | cell 4   |
```

Code above produces next output:

| header 1 | header 2 |
| -------- | -------- |
| cell 1   | cell 2   |
| cell 3   | cell 4   |


