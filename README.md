# Structure

2 groups of apps. They all have the same dependency that have both optional and required peerDependencies (@apollo/client < 4).

One is built with react 18 other with 16. In order to allow for teams to handle their own upgrades, we want the possiblilty to have 2 versions of react for a period of time.

Even in this simple case where we don't have any shared libs, using dedupe-peer-dependents brings in the wrong version of reqact to one of the apps.