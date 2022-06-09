# aws-login

Open an AWS console session for a given IAM role in an appropriate Firefox container from the command line.

## Prerequisites

- [aws-vault](https://github.com/99designs/aws-vault)
- [firefox](https://www.mozilla.org/en-GB/firefox/new/)
- firefox [multi-account-containers](https://addons.mozilla.org/en-US/firefox/addon/multi-account-containers/) addon
- firefox [open-url-in-container](https://addons.mozilla.org/en-US/firefox/addon/open-url-in-container/) addon
- [jq](https://stedolan.github.io/jq/)

## Usage

```bash
aws-login foo-account-BarRole
```

Where `foo-account-BarRole` is an IAM role you can assume in the `foo-account` AWS account using `aws-vault`, and you have a Firefox container named `foo-account`.

The tool assumes that you have your profile names structured in this `{account}-{role}` format.

## Installation

1. Clone the repo.
2. Updated your shell rc script to add the repo `bin` directory to your `PATH` variable.
