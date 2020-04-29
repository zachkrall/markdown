# markdown

generator for creating markdown files with chained javascript functions.

example:
```
/* npm install zachkrall/markdown */
const md = require('markdown')
const { writeFileSync } = require('fs')

md
.h1('markdown')
.text('generator for creating markdown files with chained javascript functions.')
.code(`
  console.log(Hello World);
`)

writeFileSync('./README.md', md.value, { encoding: 'UTF-8' })
```
