ComponentBuilder
================

A project for testing string-represented component-based language.

<h2>Grammar</h2>

1. A component can have any number of Inports (or none) and any number of Outports (or none).
2. It's possible to link two components Serially if the first's outports count is equal to the second's inports count. The resulting component has the first's inports count and the second's outports count.
3. It's possible to link two componets In Parallel without any condition. The resulting component's inports = the addition of the composites' inports, and it's outports = the addition of the composites' outports.
4. Linking In Parallel has higher priority than linking Serially.
5. Parenthesis are allowed.
6. Linking Serially is represented by cascading the two components without any seperator.
7. Linking In Parallel is represented by seperating the two components with a & sign.
8. Allowed Characters are: `digits`, `,` comma, `(`, `)`, `<`, `>`, `&`, and `whitespaces`.
9. A simple component should be represented as `<Inports_Number,Outports_Number>`.
10. The language is whitespaces insensitive, unless they occur inside a number (e.g, `15 123` instead of `15123`).
