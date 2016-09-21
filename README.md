mathjax-single-file
===================

# SGY Modifications

* Added new configuration for generating MML+TeX to SVG 
* Removed MathJax npm install
* Added wget download for MathJax to ensure we are getting the same version that this system was developed for
* Added md5 validation for downloaded mathjax archive

## Building

Download or clone this project then install dependencies:

`npm install`

Then build the specific version. Schoology is using MMLTeXSVG

`grunt MMLTeXSVG`

This will produce a minified, and non-minified file within the `dist` directory.

# Original Notes

An **experimental** MathJax build as a single file.

This built offers two example configurations -- MMMLSVG, TeXSVG -- providing

* MathML input or TeX input
* SVG output with MathJax TeX "fonts"
* extensions 
*   * MMLSVG: mml3.js, webfonts matching, AssistiveMML
*   * TeXSVG: almost all core TeX extensions
* misc. MathJax internals

See the Gruntfile for more information.

For more background, see https://github.com/mathjax/MathJax/wiki/Single-file-built
