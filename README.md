# Example
![Clubhouse Task](https://imgur.com/eSGqrRa)

```yml
steps:
  - plugins:
      - CaseyMichael/clubhouse-buildkite-status-badge#v1.2.3:
          CLUBHOUSE_API_TOKEN: value
          GITHUB_BRANCH_NAME: feature/ch17-clubhouse-ticket-name
          BUILDKITE_PIPELINE_URL: https://buildkite.com/org-name
          BUILDKITE_PIPELINE_BADGE_URL: https://badge.buildkite.com/sample.svg
```