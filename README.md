[![CircleCI](https://circleci.com/gh/giantswarm/{APP-NAME}.svg?style=shield)](https://circleci.com/gh/giantswarm/{APP-NAME}-app)

# {APP-NAME} chart

Giant Swarm offers a {APP-NAME} App which can be installed in tenant clusters.
Here we define the {APP-NAME} chart with its templates and default configuration.

**What is this app?**  
**Why did we add it?**  
**Who can use it?**  

## Installing

There are 3 ways to install this app onto a tenant cluster.

1. [Using our web interface](https://docs.giantswarm.io/reference/web-interface/app-catalog/)
2. [Using our API](https://docs.giantswarm.io/api/#operation/createClusterAppV5)
3. Directly creating the App custom resource on the Control Plane.

## Configuring

### values.yaml
**This is an example of a values file you could upload using our web interface.**
```
# values.yaml

```

### Sample App CR and ConfigMap for the Control Plane
If you have access to the Kubernetes API on the Control Plane, you could create
the App CR and ConfigMap directly.

Here is an example that would install the nginx-ingress-controller-app to
tenant cluster `abc12`:

```
# appCR.yaml

```

```
# user-values-configmap.yaml


```

See our [full reference page on how to configure applications](https://docs.giantswarm.io/reference/app-configuration/) for more details.

## Compatability

This app has been tested to work with the following tenant cluster release versions:
* 

## Limitations  

Some apps have restrictions on how they can be deployed.
Not following these limitations will most likely result in a broken deployment.
* 

## Credit

* {APP HELM REPOSITORY}
