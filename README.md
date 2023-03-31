### Notes
Description:  There are 2 Features

1) duckduckgo.feature - it has no tags
2) duckduckgoIgnore.feature - it has a single tag `@ignore`

```
@ignore
Feature: ignore duckduckgo.com
  Scenario: visiting the frontpage
    When I visit duckduckgo.com
    Then I should see a search bar
```

#### Run 3 ways

*  `npm run runFeatures` 
This should run all the features and does

*  `npm run runIgnoreOnly`
This should only run the feature tagged with `@ignore` and does

*  `npm run runFeaturesNotIgnore` 
This should run all Features but not the ignore.  This fails - none of the Features are run