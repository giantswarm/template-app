# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

- fixed: the chart label helper trims every `-`, `.` and `_` at the ends of the 63-character cut, so `helm.sh/chart` is a valid label value for any chart version; the cut of a long branch or helm-controller version could end in `.`, `_` or `--.`, and the API server refused every labelled object ([#70](https://github.com/giantswarm/template-app/issues/70)).
- changed: the chart's team annotation is the `{TEAM-NAME}` placeholder (the brace convention of `{APP-NAME}`), filled with the team's short name when a repository is created; the default Giant Swarm icon is documented as a default to replace, and the README lists every placeholder ([#66](https://github.com/giantswarm/template-app/issues/66)).
- added: Artifact Hub metadata (`artifacthub.io/license`, `artifacthub.io/links`) in the chart template ([roadmap#3940](https://github.com/giantswarm/roadmap/issues/3940)).

- changed: Regenerated `.circleci` config with `devctl gen circleci` — adopt the dynamic-config setup workflow (`config.yml` + `workflows.yml`) and bump the architect orb to v9.5.2.
- changed: `app.giantswarm.io` label group was changed to `application.giantswarm.io`

[Unreleased]: https://github.com/giantswarm/{APP-NAME}/tree/main
