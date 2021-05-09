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

<script type="text/javascript" src="https://cdnjs.buymeacoffee.com/1.0.0/button.prod.min.js" data-name="bmc-button" data-slug="caseymichael" data-color="#FFDD00" data-emoji=""  data-font="Poppins" data-text="Buy me a coffee" data-outline-color="#000000" data-font-color="#000000" data-coffee-color="#ffffff" ></script>