tide-design, Responsive design
==============================

- [Marcotte article](https://alistapart.com/article/responsive-web-design/) from 2010 describing technical elements (Fluid grids, flexible images, and media queries) and a design thinking path outside the boxed constraint of a fixed width and height.
- In a Nutshell; presentation in most relevant format at a *viewport* and **device**.
- Progressive enhancement is a thing, and it saves us the headache of designing for old or basic browsers.
- viewport **meta** tag: non-standard *de facto* method instructing browser how to render, introduced by Apple
- fluid image style in css, not fixed sizes in width and height
- different fluid effect from intrinsic size and container size instructed by 
  - **max-width:100%** intrinsic fluid element
  - **width:100%** container for element reference fluid
- media queries; directives in css, rules for environment constraints
- **breakpoint**-design is *bad*, like hard coding, and think before using
- **agnostic**-design is *good*, like responsive, always looks good
- **min-width**, minimum-width media query 

  ``@media screen and (min-width:400px){ /* style /* }``
