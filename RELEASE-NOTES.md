### Version 1.11.5 - March 23, 2015

- **Dropdown** - Fix bug where element will not blur on tab key when search selection and no selection made

### Version 1.11.2 - March 6, 2015

- **Search** - Search now uses internally [fuzzy search](https://github.com/bevacqua/fuzzysearch) as its new full text search algorithm.

### Version 1.11.0 - March 3, 2015

- **Dropdown** - Fixes issue where dropdown would not open after restoring previus value on failed `search dropdown` search
- **Search** - Fix special characters not searching correctly with local search
- **Search** - Fix a bug with `onSelect` returning `null` when `minCharacters: 0`
- **Search** - Fix a bug with `onSelect returning `null` when results retrieved from cached API query
- **Form** - Added `input[type="search"]` styles to `ui form`

### Version 1.10.3 - February 27, 2015

- **Search** - Fixes bug in category search causing item selection to sometimes produce a javascript error.

### Version 1.10.0 - February 23, 2015

- **Search** - Category search no longer displays unnecessary error message about maxResults

### UI Changes

- **Dropdown** - `search selection dropdown` will now close the menu when a `dropdown icon` is clicked
- **Dropdown** - Added new dropdown setting, `forceSelection` which forces `search selection` to a selected value on blur. Defaults to `true`.

### Version 1.8.0 - January 23, 2015

- **Search** - Search `onSelect` now recieves JSON object matching currently selected element, you can now programmatically retrieve result JSON using `.search('get result', 'query')` or `.search('get results')`. `get result` will default to current value unless specified as first parameter.
- **Search** - Greatly reduced search delay from `300ms` to `100ms`. Previous request will automatically abort `xhr` when new request made
- **Search** - Search `onSelect` and `onResultsAdd` can now cancel default actions by returning `false`.
- **Dropdown** - Dropdown no longer will not show menu when no `item` are present in menu. Dropdown will now only filter results for `ui search dropdown` #1632 **Thanks PSyton**.
- **Search** - Search results no longer hide/show when user changes tab or page loses focus

### Version 1.7.0 - January 14, 2015

- **Dropdown** - Search dropdown input can now have backgrounds. Fixes issues with autocompleted search dropdowns which have forced yellow "autocompleted" bg.
- **Dropdown** - Fix issue with search selection not correctly matching when values are not strings
- **Dropdown** - Fixes dropdown search input from filtering text values when input is inside menu, i.e "In-Menu Search"
- **Dropdown** - Fix issue with search selection not correctly creating RegExp when select values are not strings **Thanks @alufers**

### Version 1.6.0 - January 05, 2015

- **Form** - ``ui search dropdown`` inside a form has incorrect focus style

### Version 1.5.1 - January 01, 2015

- **Search** - Fixed issue with local search returning all results due to improper regexp

### Version 1.5.0 - December 30, 2014

- **Dropdown/Search** - Fixed issues with ``ui search`` and ``ui search dropdown`` using ``RegExp test`` which [advances pointer on match](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp/test) causing results to display incorrectly

### Version 1.3.0 - December 17, 2014

- **Dropdown** - Full text search now defaults to ``false``, meaning search terms will return only results beginning with letters
- **Dropdown** - Search Dropdown is now much more responsive, js improvements and input throttling added.Throttling defaults to `50ms` and can be modified with settings ``delay.search``
- **Dropdown** - Search Dropdown now correctly replaces placeholder text when backspacing to empty value
- **Dropdown** - Search Dropdown now has a callback when all results filtered ``onNoResults``
- **Dropdown** - Search dropdown will now strip html before searching values when searching html
- **Dropdown** - Search now has keyboard shortcut to open dropdown on arrow down

### Version 1.0.0 - November 24, 2014

- **Dropdown** - New dropdown type, searchable selection for large lists of choices

### Version 0.1.0 - Sep 25, 2013