You completed most of the media embedding and the basic page structure.
However, there are some issues that you need to address before the assignment is marked as complete:
Your blog post (post.html) does not follow the specification exactly.
The assignment requires you to have a single <article> containing:
an <header> with an <h1> title and a published date,
a <section> for the main body and
a <footer> with the author name and a list of tags.

You have used three separate <article> elements inside a <section>, with <h2> headings instead of an <h1> inside the article header.
Rewrite the post as one <article>, move your <h1> into that article’s header, add a <p> or <time> element for the date, and finally include a footer. Your bio.html file contains an error. You have a <head> tag appears inside the <body> (around line 10). This is invalid HTML and it causes the W3C validator to fail. Remove the stray <head> tag. The content inside it (the <h1> and image) should be inside a <header> element instead. Your index.html lacks a proper <nav> element and does not link to post.html. Your checklist claims this is done, but it is not. You need to add a <nav> with links to bio.html and post.html on index.html. Similarly, add a <nav> to bio.html that links back to index.html and post.html.

html
└── body
├── header (contains site title and nav linking to index, bio, post)
├── main
│ └── article
│ ├── header (contains h1 title and published date)
│ ├── section (the main body of the post, multiple paragraphs)
│ └── footer (contains author name and a list of tags)
├── aside (related posts or a short about-the-author blurb)
└── footer (site footer with copyright)
