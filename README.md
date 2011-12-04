#geneJS

geneJS (pronounced genesis) is a JavaScript tool that generates JavaScript code from PlantUML class diagram source.

Read [this blog post](http://blog.armaganamcalar.com/post/13644220178/weekend-run-javascript-code-generation-from-plantuml) about the motivation.

I started geneJS as a JavaScript code generator for my class diagrams, and then i thought of doing an abstraction so anyone can put in any language. For that purpose, geneJS uses the brilliant [mustache template engine](http://mustache.github.com).

geneJS parses the PlantUML source, builds an object tree based upon it and then renders it with mustache templates into JavaScript.

Since it's the product of a weekend code run, the code is as messy as it can be.

## Current version

I wanted to see if I could develop a reasonable code generator so I began from the end; coding templates and then the object tree output. The generator works fine with the functionality in the commented out, dummy object registry ( see Registry.js), but conversion from PlantUML is in its very early stages and is but a prototype.