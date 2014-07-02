Genesass
========

This is basically Sassified version of the Genesis Sample theme with quite a few of my own added functionality.

Sassification
-------------

I start using SASS, specifically SCSS a little while back and really like it.  In my head it fits much more closely with a _real programming language_ by supporting things like reusable pieces of code, mixins, variables.  It also allows you to structure your code in a _scoped_ manner making it much easier to read, share and maintian.

### Anyone up for some Bourbon?

I have also started using [Bourbon](http://bourbon.io), specifically I love the [neat](http://neat.bourbon.io/) grid layout framework.  I have not really gotten to [bitters](http://bitters.bourbon.io/) and [refils](http://refills.bourbon.io/) yet.. But in do time.

Anyway, this framework includes Bourbon and Neat directly.

You can find all of the style sheets in the 

```
scss 
```

Directory.  I highly recommend you edit the .scss style sheets then generate a new _style.css_ with the sass command.

Yes that does mean you'll have to setup your system to generate sass stylesheets.  Sorry, but that's just the way it goes.. But it really is not too hard to do..

Convert the .scss to .css by running the following commands from the child theme directory:

```
sass --watch scss/style.css:style.css
```

Or you can just do a one time conversion if you prefer.


About the Genesis style.css
---------------------------

I have basically moved the genesis-sample/style.css into the scss directory and renamed it to _genesis.scss so I can include it into the final stylesheet and get all the goodness that goes along with it.

I can then overwrite the default stylings for specific selectors with my own custom styles.

The idea is that I can update newer genesis-sample stylesheets with out having to rewrite them everytime.  This is not the most efficient what to handle stylesheets, but it should help future proof this code.

Sticky Secondary Menu
---------------------

You can add a sticky secondary menu by calling the function 

```
gs_do_secondary_sticky_menu();
```
