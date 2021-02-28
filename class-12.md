# Class 12

* ##  EJS Partials

Partials come in handy when you want to reuse the same HTML across multiple views. Think of partials as functions, they make large websites easier to maintain as you don’t have to go and change a piece of text in every page it appears in. Instead, you define that reusable bundle of code in a file andinclude it wherever you need it.

Our blog will consist of a home page which lists all the blog posts and a post page which will display a single post.

Now that we have our partials defined, we can use them in our home.ejs and post.ejs templates! In EJS, any JavaScript or non-HTML syntax you include in your templates is always surrounded by `<% %>` delimiters (you could change these delimiters if you really wanted to).

As you can see creating and including partials is very straightforward with EJS. I’ve intentionally left in some placeholders such as LIST_OF_POSTS, POST_TITLE, POST_AUTHOR, and POST_CONTENT so that we can take a look at how we can pass data from our Node + Express application to our views in the next section.

