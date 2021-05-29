# Clubhouse Buildkite Status Badge Plugin
![GitHub release (latest by date)](https://img.shields.io/github/v/release/CaseyMichael/clubhouse-buildkite-status-badge-buildkite-plugin)

A [Buildkite plugin](https://buildkite.com/docs/agent/v3/plugins) that adds a branch specific buildkite status badge to a task on a [Clubhouse](https://clubhouse.io/) ticket

![Clubhouse Task](https://i.imgur.com/1NTfX3Y.png)

## Example
The following pipeline will add a branch specific buildkite status badge to a task for the Clubhouse ticket `ch17`:

```yml
steps:
  - plugins:
      - caseymichael/clubhouse-buildkite-status-badge#v0.0.5:
          CLUBHOUSE_API_TOKEN: "CLUBHOUSE-API-TOKEN"
          BUILDKITE_BRANCH: "feature/ch17-clubhouse-ticket-name"
          REPOSITORY_NAME: "repository-name"
          BUILDKITE_PIPELINE_URL: "https://buildkite.com/org-name"
          BUILDKITE_PIPELINE_BADGE_URL: "https://badge.buildkite.com/sample.svg"
```

## Configuration

### `CLUBHOUSE_API_TOKEN` (Required, string)
The generated API key to access Clubhouse.

### `BUILDKITE_BRANCH` (Required, string)
The branch name that must contain the clubhouse id.

### `REPOSITORY_NAME` (Required, string)
The repository name, useful for when a single clubhouse ticket might have branches in several repositories. This adds an informational badge with the repository name.

### `BUILDKITE_PIPELINE_ULR` (Required, string)
The buildkite pipeline url for formatting the buildkite badge.

### `BUILDKITE_PIPELINE_BADGE_URL` (Required, string)
The buildkite pipeline badge url for displaying the badge.

## Developing
To run the tests:

```shell
docker-compose run --rm tests
```

## Contributing
1. Fork the repo
2. Make the changes
3. Run the tests
4. Commit and push your changes
5. Send a pull request

<a href="https://www.buymeacoffee.com/caseymichael"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=caseymichael&button_colour=FFDD00&font_colour=000000&font_family=Poppins&outline_colour=000000&coffee_colour=ffffff"></a>