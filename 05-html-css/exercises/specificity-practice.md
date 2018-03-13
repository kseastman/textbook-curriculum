## Specificity Examples: Test Yourself

It’s easier to calculate the specificity using the first method. Let’s find out, how it actually is done.

| Question | Selector     | Specificity
| :------------- | :------------- | :------------- |
| A      | `* { }`  |    |
| B      | `li.cool { } ` |    |
| C      | `li { }`  |    |
| D      | `li::first-line { }`  |    |
| E      | `ul li { }`  |    |
| F      | `ul ol+li { }` |    |
| G      | `h1 + *[rel=up] { }` |    |
| H      | `ul ol li.red { }` |    |
| I      | `li.red.level { }` |    |
| J     | `style=””` |    |
| K     | `p { }` |    |
| L     | `div p { }` |    |
| M     | `.ada { }` |    |
| N     | `div p.ada { }` |    |
| O     | `#grace { }` |    |
| P     | `body #grace.ada p { }` |    |
