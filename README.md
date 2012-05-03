ComponentBuilder
================

A project for checking string-represented component-based language.

<h2>Grammar</h2>

1. A component can have any positive number of Inports (including zero) and any number of Outports (including zero).
2. It's possible to link two components Serially if the first's outports count is equal to the second's inports count. The resulting component has the first's inports count and the second's outports count.
3. It's possible to link two componets In Parallel without any condition. The resulting component's inports count = the addition of the composites' inports counts, and it's outports count = the addition of the composites' outports count.
4. Linking In Parallel has a higher priority than linking Serially.
5. Allowed Characters are: `digits`, `,` comma, `(`, `)`, `<`, `>`, `&`, and `whitespaces`.
6. A simple component should be represented as `<Inports_Number,Outports_Number>`.
7. A token is one of the following: `Number`, `,` comma, `<`, `>`, `(`, `)`, and `&`.
8. Parenthesis are allowed between simple and composite components, and cannot appear.
9. Linking Serially is represented by cascading the two components without any seperator.
10. Linking In Parallel is represented by seperating the two components with a & sign.
11. All white spaces are removed while checking.