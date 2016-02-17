##Problem 1
Research about the following HTML tags and explain their semantics:

`<strong>` : gives text strong importance, and is typically displayed in bold.

`<em>` : gives text strong importance, and is typically displayed in bold.

`<blockquote>` :  indicates that the enclosed text is an extended quotation

`<q>` : indicates that the enclosed text is a short inline quotation

`<abbr>` : represents an abbreviation and optionally provides a full description for it

`<cite>` : represents a reference to a creative work

`<dfn>` : represents the defining instance of a term

`<address>` : supplies contact information for its nearest `<article>` or `<body>` ancestor; in the latter case, it applies to the whole document

`<ins>` : represents a range of text that has been added to a document

`<del>` : represents a range of text that has been deleted from a document

`<s>` : renders text with a strikethrough, or a line through it



##Problem 2
Explain why do we need `<thead>`, `<tbody>` and `<tfoot>`?

Those are elements to create a table (`<Table>` represents data in two dimensions or more). They are optionals, but must be useful for complex table.
`<thead>` is the firtst row of the table wher there is the "title" of each column.
`<tbody>` is the other rows of the table, below the `<thead>`. Each row is create with a `<tr>` element.
`<tfoot>` is the last row of the table.

