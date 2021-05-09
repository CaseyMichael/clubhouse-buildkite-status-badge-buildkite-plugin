# Clubhouse Buildkite Status Badge Plugin
A [Buildkite plugin](https://buildkite.com/docs/agent/v3/plugins) that adds a branch specific buildkite badge to a clubhouse ticket
![Clubhouse Task](https://imgur.com/eSGqrRa.png)

## Example

The following pipeline will add a buildkite badge to the Clubhouse ticket `ch17`:

```yml
steps:
  - plugins:
      - CaseyMichael/clubhouse-buildkite-status-badge#v1.2.3:
          CLUBHOUSE_API_TOKEN: value
          GITHUB_BRANCH_NAME: feature/ch17-clubhouse-ticket-name
          BUILDKITE_PIPELINE_URL: https://buildkite.com/org-name
          BUILDKITE_PIPELINE_BADGE_URL: https://badge.buildkite.com/sample.svg
```