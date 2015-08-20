# Sass Structure
> A base sass structure to modularize your sass.

### Directory Structure

```

styles/
|
|-- modules                # Common modules
| |-- _all.scss            # Include to get all modules
|
|-- partials               # Partials
| |-- _base.scss           # imports for all mixins + global project variables
| |-- _general.scss        # general scss not specific. Make new files for to be specific
|
|-- utilities              # Utilities
| |-- _all.scss            # Include to get all utilitie files
| |-- _mqs.scss            # Media Queries - from Zurb *
| |-- _normalize.scss      # Normalize for css reset
| |-- _rem-calc.scss       #
|
|-- vendors                # CSS or Sass from other projects
| |-- _all.scss            # Include to get all vendor sass files
|
|-- _variables.scss        # global variables set here
|-- main.scss              # primary Sass file

```
* Media Queries mixins [Zurb](http://foundation.zurb.com/docs/media-queries.html)
* [Normalize](https://necolas.github.io/normalize.css/) converted to sass by [John Albin](https://github.com/JohnAlbin/normalize-scss)