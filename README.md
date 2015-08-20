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
| |-- _normalize.scss      # Normalize for css reset *
| |-- _rem-calc.scss       # Rem-Calc functions - from Zurb *
|
|-- vendors                # CSS or Sass from other projects
| |-- _all.scss            # Include to get all vendor sass files
|
|-- _variables.scss        # global variables set here
|-- main.scss              # primary Sass file

```
* *Media Queries mixins [Zurb](http://foundation.zurb.com/docs/media-queries.html)
* *[Normalize](https://necolas.github.io/normalize.css/) converted to sass by [John Albin](https://github.com/JohnAlbin/normalize-scss)
* *Rem-calc functions pulled from [Zurb](https://github.com/zurb/foundation/blob/master/scss/foundation/_functions.scss)



## About rem-calc()

Syntax, allows to optionally calculate on a different base value to counter compounding effect of rem's.

- Call with 1, 2, 3 or 4 parameters, 'px' is not required but supported:`rem-calc(10 20 30px 40);`
- Space delimited, if you want to delimit using comma's, wrap it in another pair of brackets `rem-calc((10, 20, 30, 40px));`
- Optionally call with a different base (eg: 8px) to calculate rem. `rem-calc(16px 32px 48px, 8px);`
- If you require to comma separate your list `rem-calc((16px, 32px, 48), 8px);`