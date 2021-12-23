# linting-via-github-action

This repository contains Github Actions differant types of linting like...

1. hadolint
2. yamllint
3. xmllint

You can use any of the build workflow as per your project requirement and linting you want to perform accordingly.

* hadolint 

In hadolint action ,if you want ignore some error , you can use ignore section as follows

- name: Hlint
  uses: hadolint/hadolint-action@v1.5.0
  with:
    dockerfile: Dockerfile
    ignore: DL3007 DL3025 DL4003

You can refer this https://github.com/hadolint/hadolint#rules for rules of dockerfile.