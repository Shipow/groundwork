# Contributing to GroundworkCSS

Looking to contribute something to Groundwork? **Here's how you can help.**



## Reporting issues

1. **Create an isolated and reproducible test case.** Be sure the problem exists in the Groundwork code with a [reduced test case](http://css-tricks.com/reduced-test-cases/) that should be included in each bug report.
2. **Include a live example.** Make use of jsFiddle or Codepen to share your isolated test cases.
3. **Share as much information as possible.** Include operating system and version, browser and version, version of Groundwork, etc. where appropriate. Also include steps to reproduce the bug.



## Key branches

- `master` is the latest, deployed version
- `grid` is the stand-alone grid system branch
- `X.XX.X-wip` branches are the official work in progress branches for the next releases. All pull requests should be submitted against the appropriate branch



## Pull requests

- Submit all pull requests against the appropriate `*-wip` branch for easier merging
- CSS changes must be done in the .scss files first, never the compiled files
- HTML changes must be done in the .jade template files first, never the compiled files
- When modifying any source files (.scss, .jade, coffee, etc.), always recompile and commit the compiled files by using the Grunt tasks `grunt build`
- Try not to pollute your pull request with unintended changes -- keep them simple and small (minimize unecessary diffs)
- Try to share which browsers your code has been tested in before submitting a pull request



## Coding standards: HTML

- Two spaces for indentation, never tabs
- Double quotes only, never single quotes
- Always use proper indentation
- Use tags and elements appropriate for an HTML5 doctype (e.g., self-closing tags)



## Coding standards: CSS

- Multiple-line approach (one property and value per line)
- Always a space after a property's colon (.e.g, `display: block;` and not `display:block;`)
- End all lines with a semi-colon
- For multiple, comma-separated selectors, place each selector on it's own line
- Use of .scss comments are okay when necessary ("//"), but do not use CSS comments ("/* */")
- Attribute selectors, like `input[type="text"]` should always wrap the attribute's value in double quotes, for consistency and safety (see this [blog post on unquoted attribute values](http://mathiasbynens.be/notes/unquoted-attribute-values) that can lead to XSS attacks)



## License

By contributing your code, you agree to license your contribution under the terms of the MIT License:
- http://opensource.org/licenses/mit-license.html
