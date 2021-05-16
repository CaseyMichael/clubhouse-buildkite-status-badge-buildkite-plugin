# Clubhouse Release Plugin

## Example

The following pipeline will add story links for all of the branches that were merged into the release branch. 

```yml
steps:
  - plugins:
      - CaseyMichael/clubhouse-release#v1.0.0:
          CLUBHOUSE_API_TOKEN: "value"
          GITHUB_API_TOKEN: "value"
          CLUBHOUSE_RELEASE_STORY_ID: 12451
          GITHUB_OWNER: "org"
          GITHUB_REPO: "repo-name"
          GITHUB_BASE_BRANCH: "production"
          GITHUB_RELEASE_BRANCH: "staging"

```

<a href="https://www.buymeacoffee.com/caseymichael"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=caseymichael&button_colour=FFDD00&font_colour=000000&font_family=Poppins&outline_colour=000000&coffee_colour=ffffff"></a>