[![CircleCI](https://dl.circleci.com/status-badge/img/gh/giantswarm/{APP-NAME}/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/giantswarm/{APP-NAME}/tree/main)
[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/giantswarm/{APP-NAME}/badge)](https://securityscorecards.dev/viewer/?uri=github.com/giantswarm/{APP-NAME})

[Guide about how to manage an app on Giant Swarm](https://handbook.giantswarm.io/docs/dev-and-releng/app-developer-processes/adding_app_to_appcatalog/)

## Creating a repository from this template

A repository is created from this template by the repository set-up engine (`devctl`), which replaces the
placeholders below and pushes the result as the first commit. When copying by hand, replace them yourself.

| Placeholder | Where | Replaced with |
|---|---|---|
| `{APP-NAME}` | the chart directory `helm/{APP-NAME}`, `Chart.yaml`, `values.yaml`, `.abs/main.yaml`, `CHANGELOG.md`, this README | the repository name |
| `{TEAM-NAME}` | the `io.giantswarm.application.team` annotation in `Chart.yaml` | the owning team's short name, e.g. `shield` for team-shield |
| `{APP HELM REPOSITORY}` | this README | the upstream Helm repository the chart is based on |

The chart ships with the default Giant Swarm icon (`https://s.giantswarm.io/app-icons/giantswarm/1/light.svg`),
so that the first build passes the icon checks. It is a default, not a placeholder: replace it with the app's
own icon by adding it to [web-assets](https://github.com/giantswarm/web-assets) and setting the final URL as
`icon` in `Chart.yaml`.

Remove this section from the README of the created repository.

# {APP-NAME} chart

Giant Swarm offers a {APP-NAME} App which can be installed in workload clusters.
Here, we define the {APP-NAME} chart with its templates and default configuration.

**What is this app?**

**Why did we add it?**

**Who can use it?**

## Installing

There are several ways to install this app onto a workload cluster.

- [Using GitOps to instantiate the App](https://docs.giantswarm.io/tutorials/continuous-deployment/apps/add-appcr/)
- By creating an [App resource](https://docs.giantswarm.io/reference/platform-api/crd/apps.application.giantswarm.io) using the platform API as explained in [Getting started with App Platform](https://docs.giantswarm.io/tutorials/fleet-management/app-platform/).

## Configuring

### values.yaml

**This is an example of a values file you could upload using our web interface.**

```yaml
# values.yaml

```

### Sample App CR and ConfigMap for the management cluster

If you have access to the Kubernetes API on the management cluster, you could create the App CR and ConfigMap directly.

Here is an example that would install the app to workload cluster `abc12`:

```yaml
# appCR.yaml

```

```yaml
# user-values-configmap.yaml

```

See our [full reference on how to configure apps](https://docs.giantswarm.io/tutorials/fleet-management/app-platform/app-configuration/) for more details.

## Compatibility

This app has been tested to work with the following workload cluster release versions:

- _add release version_

## Limitations

Some apps have restrictions on how they can be deployed.
Not following these limitations will most likely result in a broken deployment.

- _add limitation_

## Credit

- {APP HELM REPOSITORY}
