# easy-peasy-blog
A vanila #javascript blog template/engine, which takes #html or markdown or even a  doc file with some delimiter and generates a static site. No frameworks.Just plain HTML, CSS & javascript. 

## Idea (An agent for each step):
- Layout: Use template literals for layouts. These functions accepts data as props and returns html string
- Parser: Parser parses the markdown files and passes the data to the layouts.
- Writer: Writer writes the output from the layout to a html file
- Watcher: Watches for file changes (used to create a new build on file change)
- Later we will need even more agents, like - Linker (links files), Paginator (paginates), RSS (Generates RSS feed and sitemap), PWA generator (Generates PWA)
- Manager: Manages all the agents.

## Plan - v0

- [ ] Setup a dev server, node 
- [ ] Create HTML layout (start with a static page) & set of available tags to auto insert in the layout
- [ ] Setup markdown parser & get the tagged content
- [ ] Auto insert tagged content in the layout & create a static page
- [ ] Setup build config & build command
- [ ] First Release

## Plan - Next

- [ ] Transpile js, productionise (minify, uglify) HTML, CSS
- [ ] Add support for images
- [ ] Add support for doc file blogs (write blogs in a doc file with tags)
- [ ] Theme customisation
