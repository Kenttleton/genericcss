# Genericcss

Genericcss is an implementation of style sheets using the theory of [Atomic Design by Brad Frost](http://atomicdesign.bradfrost.com/). I highly recommend his book
 if you have never read it. Genericcss for the most part falls under the Atom level of the Atomic design theory.

The development of this implementation started from a need to boil down the styling for use with multiple CMS platforms meaning standardization and generic use
 cases were needed. Combine this with simple language allows for non-developers, for those who have Marketing or management making changes to the copy, who want
 to make style changes can add, change, or remove keywords to style page elements without developer intervention, if the CMS platform supports added styles. For
 those platforms that don't support CSS classes through the Admin GUI; this repository also functions as a Boostrap-esque developer tool for faster development
 and styling.

Codebase reduction and reuse was another focus for this project. By implementing a generic library of style sheets this shrank the standard style sheet from 100s
 of lines of code per page to 150 lines or less. This differs from current web standards of short CSS classes and long style sheets to longer CSS class names to
 smaller style files. Smaller style files transmit faster over the internet and even sped up page loads.

Some beneficial features include:
- [CSS Grid](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout) support; I prefer 2D layouts as apposed to faked 2D using flex or Bootstrap.
- Most styling is HTML tag agnostic, e.g. the Button class will handle `<div>` and `<a>` as buttons.
- Dynamic color pallettes, if the color in the class matches a color on the Colors style sheet it'll work.
- Expandable. From this base Molecules, Organisms, etc. can be built with access to sub functions as needed by a simple `@import`.

Notes:
- IE and Edge are not 100% verified to work in current version
- In-depth documentation using [DocumentCSS](https://documentcss.com/) coming soon.
- [Yarn](https://yarnpkg.com/en/) management/workflow and a lightweight bundler/minification package like [Parcel](https://parceljs.org/) coming soon.


## Conclusion
Due to the discovery of better flex based frameworks like [UIKit](https://getuikit.com/) that were extensible and light and the lack of legacy support for CSS Grid in IE this project was ultimate abandoned for more compatible alternatives. Development may continue in the future when support for CSS Grid is mainstream and 3 iterations before current versions.  