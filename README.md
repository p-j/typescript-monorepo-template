# Typescript Monorepo Template

This template is intended for OSS Typescript based projects and is centered around a few tools:

- **yarn** for dependency management and running tasks like `test` or `publish`
- **lerna** for running package level commands
- **changeset** for managing changelog generation, and release creation
- **codecov** for code coverage

It's a template that I tend to use for my own projects like

- [EAPI](https://github.com/p-j/eapi): a suite of middleware & utility to build scalable cloudflare workers backend/proxy
- [GeocodeJSON](https://github.com/p-j/geocodejson): a suite of adapter & utility for geocoding API that maps to [GeocodeJSON](https://github.com/geocoders/geocodejson-spec/tree/master/draft) resutls

## How to use this template

_AKA: "Note to self"_

- Get started by clicking [Use this template](https://github.com/p-j/typescript-monorepo-template/generate)
- Update the required files as [described below](https://github.com/p-j/typescript-monorepo-template#what-you-need-to-change)
- Use `yarn` for dependencies as this template make use of [Yarn Workspaces](https://classic.yarnpkg.com/en/docs/workspaces/)
- Browse the scripts to understand how `lerna` `changeset` and `yarn` play together to `build` `test` and `publish` releases.
- [Setup integration](https://github.com/settings/installations) with [Changeset](https://github.com/atlassian/changesets)
- [Setup integration](https://github.com/settings/installations) with [CodeCov](https://github.com/codecov)
- Add the necessary `SECRETS` (`NPM_TOKEN` & `CODECOV_TOKEN`)

## What you need to change

- `package.json`: change project name, author etc...
- `LICENSE`: change the copyright holder
- `CODE_OF_CONDUCT.md`: change the contact address in the `Enforcement` paragraph
- `.github/workflows/release.yml`: change the guard to your repository name
- `.changeset/config.json`: change the repository name
