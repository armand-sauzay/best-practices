# Pre commit checks 101

You need to add __2__ files:
- __.pre-commit-config.yaml__: defines the checks you want to run
- __.commitlintrc.yaml__: defines the npm package you use for pre commits.

``` yaml
# .commitlintrc.yaml
extends:
  - "@open-turo/commitlint-config-conventional"
```


``` yaml
# .pre-commit-config.yaml
repos:
  - repo: https://github.com/pre-commit/pre-commit-hooks
    rev: v2.3.0
    hooks:
    -   id: check-yaml
    -   id: end-of-file-fixer
    -   id: trailing-whitespace
  - repo: https://github.com/alessandrojcm/commitlint-pre-commit-hook
    rev: v8.0.0
    hooks:
      - id: commitlint
        stages: [commit-msg]
        additional_dependencies: ["@open-turo/commitlint-config-conventional"]"
```

Once you added those files, you can try adding a commit, the pre commit checks defined will make sure that:
- yaml files are correctly formatted
- files have an extra empty line at the end (this is considered best practice as some systems fail when this condition is not met)
- get rid of trailing whitespaces
- make sure that the commits follow the [conventinal commits](https://www.conventionalcommits.org/en/v1.0.0/) format.
