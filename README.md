# Clubhouse Buildkite Status Badge Plugin
A [Buildkite plugin](https://buildkite.com/docs/agent/v3/plugins) that adds a branch specific buildkite badge to a task on a [Clubhouse](https://clubhouse.io/) ticket
![Clubhouse Task](https://imgur.com/eSGqrRa.png)

## Example

The following pipeline will add a buildkite badge to a task for [Clubhouse](https://clubhouse.io/) ticket `ch17`:

```yml
steps:
  - plugins:
      - CaseyMichael/clubhouse-buildkite-status-badge#v1.2.3:
          CLUBHOUSE_API_TOKEN: value
          GITHUB_BRANCH_NAME: feature/ch17-clubhouse-ticket-name
          BUILDKITE_PIPELINE_URL: https://buildkite.com/org-name
          BUILDKITE_PIPELINE_BADGE_URL: https://badge.buildkite.com/sample.svg
```

<a href="https://www.buymeacoffee.com/caseymichael"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=caseymichael&button_colour=FFDD00&font_colour=000000&font_family=Poppins&outline_colour=000000&coffee_colour=ffffff"></a>