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
  ```
  @media screen and (min-width:400px){  
  /* style /*  
  }
  ```
 - There are tools for vendor prefixes
 - There are many tools for many things
   - [media queries](https://www.w3.org/TR/?filter-tr-name=media+queries)
   - [living standard](https://html.spec.whatwg.org/multipage/)
   - [can i use](https://caniuse.com)

***

HTML
====

- **marking up** elements
- **void** elements
  - *param* is now obsolete, see *can i use* and *living standard*
- ``<!doctype html>`` or ``<!DOCTYPE html>`` 
  - HTML5 doctype declaration 
- ``<html lang="en">``
  - **root** tag with **lang** attribute
- ``<head>``
  - **head** section
- ``<meta charset="utf-8" />``
  - Specified in a **meta** tag, character encoding should always be **utf-8**, but can be something else
- **conscientious** vs. **laxed** markup, a feature of HTML5
  - ``<link href="CSS/main.css" rel="stylesheet" type="text/css" />``
  - ``<link href=CSS/main.css rel=stylesheet >``
- More tools
  - [boilerplate](https://html5boilerplate.com)
    - ``brew install nvm``
    - ``nvim ~/.zshrc``
      ```
      export NVM_DIR="$HOME/.nvm"
      . "$(brew --prefix nvm)/nvm.sh"
      ```
    - ``source ~/.zshrc``
    - ``nvm - version``
    - ``nvm install node``
      ```
      npx create-html5-boilerplate new-site
      cd new-site
      npm install
      npm run start
      ```
  - **[or simply clone repo](https://github.com/h5bp/html5-boilerplate-template)**
  - [validate html](https://validator.w3.org)

## HTML5

- HTML5 allow multiple elements in a singel **a** tag
- semantics
  - sectioning
    - **main**, there can be only one and everything goes here (except repeated content)
    - **section**, is not for styling, but think of layout
    - **nav**, is for navigation links and a better choice than **ul** and **li**
    - **article**, nested article elements are related, and article is self containing isolated from the rest of the page
    - **aside**, for content related but not part of page context
    - **header**, everything can have a header
    - **footer**, everything can have a footer (but the specs point to **address** for
  - grouping
  - text-level semantics
- **outline** algorithm, theoretical, future, but there is meaning for  
[\- \[outliner tool 1\]\(https://gsnedders.html5.org/outliner/\)\]: #  
  - [outliner tool 2](https://hoyois.github.io/html5outliner/)

