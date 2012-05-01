ComponentBuilder
================

A project for testing string-represented component-based language.

<h2>Grammar</h2>

1. A component can have any number of Inports (or none) and any number of Outports.
2. It's possible to link two components Serially if the first's outports count is equal to the second's inports count.
3. It's possible to link two componets In Parallel without any condition.
4. Linking In Parallel has higher priority than linking Serially.
5. Parenthesis are allowed.
6. Linking Serially is represented by cascading the two components without any seperator.
7. Linking In Parallel is represented by seperating the two components with a & sign.