+++
categories = ["micro"]
date = "2007-07-17T22:40:45"
tags = ["tumblr"]
title = "Building Open Library, we faced a difficult new technical problem"
+++

{{<blockquote cite="About the technology" citelink="http://demo.openlibrary.org/about/tech">}}
  <p>Building Open Library, we faced a difficult new technical problem. We wanted a database that could hold tens of millions of records, that would allow random users to modify its entries and keep a full history of their changes, and that would hold arbitrary semi-structured data as users added it. Each of these problems had been solved on its own, but nobody had yet built a technology that solved all three together. So we created ThingDB (tdb), a new database framework that gives us this flexibility. ThingDB stores a collection of objects, called &ldquo;things&rdquo;. For example, on the Open Library site, each page, book, author, and user is a thing in the database. Each thing then has a series of arbitrary key-value pairs as properties.</p>
{{</blockquote>}}
