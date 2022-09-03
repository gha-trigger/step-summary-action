# step-summary-action

GitHub Actions to show [gha-trigger](https://gha-trigger.github.io/)'s [step summary](https://docs.github.com/en/actions/using-workflows/workflow-commands-for-github-actions#adding-a-job-summary)

![image](https://user-images.githubusercontent.com/13323303/187903524-260b805c-5d02-4e29-ad14-8a4320f28071.png)

## Example

```yaml
on:
  workflow_dispatch:
    inputs:
      data:
        required: true
jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - uses: gha-trigger/step-summary-action@main
        with:
          data: ${{inputs.data}}
```

## Inputs

- `data`: gha-trigger's workflow_dispatch event input `data`

## Outputs

Nothing.

## LICENSE

[MIT](LICENSE)
