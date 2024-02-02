# $${\color{lightgreen}TestRail \space - \space Usage \space - \space Tips \space \space and \space \space Tricks}$$

<br>

# Advanced Search Options

When you enter a search term into TestRail’s search box (in the upper-right corner of the user interface), TestRail will automatically search through all project entities, including test cases, runs, and suites. TestRail will also search through any custom field that you’ve added to the test case and test results.

But you can also just enter the ID of any entity to directly jump to it. For example, if a colleague is asking you to take a look at test case #15, you can directly jump to it by entering C15 into the search box. Likewise, to jump to the test suite #7, simply enter S7.

Each entity uses a different symbol in front of the ID. There is a complete list of all supported entities in the graphic above. You can find the ID of an entity next to its title on most pages.

<br>

$${\color{green}**────────────────────────────────────────────────────────**}$$

<br>

# Editor Formatting Reference

## Italics and Bolds

There are multiple ways to emphasize words using \*asterisks* or \_underscores_.
- A single \*asterisk* or \_underscore_ will \_ *italicize the text*_.
- Two \*\*asterisks*\* or \_\_underscores_\_ will \__ **bold the text**__.
- Three \*\*\*asterisks*\*\* or \_\_\_underscores_\_\_ will \_\_\_***make the text bolded AND italicized***_\_\_.

## Code and Preformatted Text

To make a code block, indent four spaces. The text will be wrapped in tags and displayed in a monospaced typeface. The first four spaces will be stripped off, but all other white spaces will be preserved. If code blocks are embedded in text blocks, they require an empty line before and after.

Example:
``` groovy
        Hello there!
        This code is in a formatted code block
```

## Code Spans

Use backticks to create an inline \<code> span. (The backtick key is in the upper left corner of most keyboards.) Like code blocks, code spans will be displayed in a monospaced typeface. Markdown and HTML will not work within them. 

Example:
``` groovy
`Example Text`
```

## Links

There are two ways to write links. The link definitions can appear anywhere in the document — before or after the place where you use them.

Example:
``` groovy
Here’s an inline link to  [Google](https://www.google.com/)
Here’s a reference-style link to  [Google][1] . [1]:https://www.google.com/
```

## Headers

You can underline text to make the two top-level headers. The number of = or – signs does not matter. You can get away with just one. But using enough to underline the text makes your titles look better in plain text.

Example:
``` groovy
Header 1
=======
Header 2
———–
```

You can also use hash marks for several levels of headers. The closing # characters are optional.

Example:
``` groovy
# Header 1 #

## Header 2 ##

### Header 3 ###
```

## Horizontal Rules

You can insert a horizontal rule \<hr/> by putting three or more hyphens, asterisks, or underscores on a line by themselves. 

Example:
``` groovy
Rule #1
---


Rule #2
*******


Rule #3
___
```

You can also use spaces between the characters:

Example:
``` groovy
Rule #4
  - - - -
```

All of these examples produce the same output.

## Simple Lists

- ### Bulleted List:

  Example:
``` groovy
–   Use a minus sign for a bullet
> +   Or plus sign
*   Or an asterisk
```

- ### Numbered List:

  Example:
``` groovy
1.   Numbered lists are easy

2.   Markdown keeps track of the numbers for you

7.   So this will be item 3.
```

- ### Double-Spaced List:

  Example:
``` groovy
–   This list gets wrapped in <p> tags




–   So there will be extra space between items
```

## Blockquotes

Blockquotes are indented.

Add a > to the beginning of any line to create a blockquote.

Example:
``` groovy
>  The syntax is based on the way email programs
>  usually do quotations. You don’t need to hard-wrap
>  the paragraphs in your blockquotes, but it looks much nicer if you do.
```

## Images

Images are exactly like links, but they have an exclamation point in front of them. The word in square brackets is the alt text which appears if the browser can’t show the image. 

``` groovy
![Valid XHTML](https://w3.org/Icons/valid-xhtml10).
```

## Tables

The first line specifies the table header and column alignments. The alignments are determined by colon characters in the respective header cells at the beginning/end of the cells. The following alignments are supported:

| `Header Syntax` | `Header Alignment` |
| :---: | --- |
| \:Header | Left-aligned (default) |
| \:Header: | Centered |
| Header: | Right-aligned |

The table cells themselves support a limited set of rich-text formatting. The following features are supported inside a table cell:
- Code Spans
- Links

Tables can be formatted as follows:

``` groovy
||| :Header 1 | :Header 2| :Header 3 | :Header 4
|| Row 1 .. | R1H2 | R1H3 | R1H4
|| Row 2 .. | R2H2 | R2H3 | R2H4
```

## Advanced Lists

You can put other Markdown blocks in a list. Simply indent four spaces for each nesting level:

``` groovy
1. Lists in a list item:
    - Indented four spaces.
        * indented eight spaces.
    - Four spaces again.
2. Multiple paragraphs in a list items:
    It's best to indent the paragraphs four spaces
    You can get away with three, but it can get
    confusing when you nest other things.
    Stick to four.
3. Preformatted text in a list item:

        Skip a line and indent eight spaces.
        That's four spaces for the list
        and four to trigger the code block.
```

## Advanced Blockquotes

You can put other Markdown blocks in a blockquote. To do so, add a > followed by a space.

Paragraph breaks in a blockquote:

``` groovy
> The `>` on the blank lines is required

> to create a single blockquote.

>

> If you leave out the extra `>`

> you will end up with

> two distinct blockquotes.
```

<br>

$${\color{green}**────────────────────────────────────────────────────────**}$$

<br>

# Keyboard Shortcuts & Hotkeys

TestRail supports keyboard shortcuts for important and frequently used actions such as editing/saving objects, adding results/comments and attachments, and navigating between cases or tests.

## Common Shortcuts

| `General` |  |
| :---: | --- |
| **\[Enter]** | Submits a dialog (unless a text control is currently focused). Applies to all dialogs in TestRail (e.g. the Add Result dialog). |
| **\[Cmd + S]** | Submits a form. This applies to all forms in TestRail (for example, the page that opens when you edit a test case). |

## Shortcuts Reference

| `Cases` |  |
| :---: | --- |
| **\[E]** | Opens the form to edit the test case |
| **\[J]** | Navigates to the next case in the test suite/case repository |
| **\[K]** | Navigates to the previous case in the test suite/case repository |
| **\[Cmd + ⬆]** | Moves the current step up (with separated steps) |
| **\[Cmd + ⬇]** | Moves the current step down (with separated steps) |
| **\[Cmd + .]** | Adds a new step after the current step (with separated steps) |
| **\[Alt + .]** | Adds a new step after the last step (with separated steps) |

<br>

| `Dashboard` |  |
| :---: | --- |
| **\[P]** | Opens the form to add a new project |

<br>

| `Milestones` |  |
| :---: | --- |
| **\[E]** | Opens the form to edit the milestone |

<br>

| `Plans` |  |
| :---: | --- |
| **\[E]** | Opens the form to edit the test plan |

<br>

| `Projects` |  |
| :---: | --- |
| **\[E]** | On the project overview page, opens the form to edit the project |

<br>

| `Runs` |  |
| :---: | --- |
| **\[A]** | Opens the **Assign To** dialog (for the currently selected tests, if any) |
| **\[E]** | Opens the form to edit the test run |
| **\[R]** | Opens the **Add Result** dialog (for the currently selected tests, if any) |
| **\[J]** | With active three-pane view: Navigates to the next test in the run |
| **\[K]** | With active three-pane view: Navigates to the previous test in the run |
| **\[P]** | With active three-pane view: Passes the currently selected test |
| **\[Q]** | Toggles the three-pane view (if previously active) |
| **\[Alt + M]** | With active three-pane view, activates the comment field for the currently selected test (**CMD + Enter** submits the comment) |
| **\[Alt + R]** | With active three-pane view, opens the **Add Result** dialog for the currently selected test |

<br>

| `Suites` |  |
| :---: | --- |
| **\[C]** | Opens the forms to add a new test case to the suite |
| **\[CMD + .]** | Activates the inline-add feature to add a new test case to the current section (subgroups and selected view modes only) |
| **\[E]** | Opens the form to edit the test suite (or opens the **Edit Description** dialog if using the single-suite project mode) |
| **\[R]** | Opens the forms to add a new test run for the suite|
| **\[S]** | Opens the dialog to add a new section to the end of the suite |
| **\[CMD + S]** | Opens the dialog to add a new subsection to the current section (subgroups and selected view modes only) |
| **\[J]** | With active three-pane view: Navigates to the next case in the test suite/case repository |
| **\[K]** | With active three-pane view: Navigates to the previous case in the test suite/case repository |
| **\[Q]** | Toggles the three-pane view (if previously active) |

<br>

| `Tests` |  |
| :---: | --- |
| **\[A]** | Opens the **Assign To** dialog to assign the test |
| **\[C]** | Navigates to the test case of the test |
| **\[E]** | Opens the form to edit the test case of the test |
| **\[J]** | Navigates to the next test in the test run |
| **\[K]** | Navigates to the previous test in the test run |
| **\[M]** | Opens the **Add Comment** dialog to add a comment |
| **\[R]** | Opens the **Add Test Result** dialog to add a test result |

<br>

| `Administration` |  |
| :---: | --- |
| **\[U]** | Add a new user on the administration **Users** tab |
| **\[M]** | Add multiple users on the administration **Users** tab |












