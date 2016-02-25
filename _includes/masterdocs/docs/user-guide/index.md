
* TOC
{:toc}

The user guide is intended for anyone who wants to run programs and services on an existing Kubernetes cluster.  Setup and administration of a Kubernetes cluster is described in the [Cluster Admin Guide](/{{page.version}}/docs/admin/). The [Developer Guide](/{{page.version}}/docs/devel/) is for anyone wanting to either write code which directly accesses the Kubernetes API, or to contribute directly to the Kubernetes project.

Please ensure you have completed the [prerequisites for running examples from the user guide](/{{page.version}}/docs/user-guide/prereqs).

## Quick walkthrough

1. [Kubernetes 101](/{{page.version}}/docs/user-guide/walkthrough/)
1. [Kubernetes 201](/{{page.version}}/docs/user-guide/walkthrough/k8s201)

## Thorough walkthrough

If you don't have much familiarity with Kubernetes, we recommend you read the following sections in order:

1. [Quick start: launch and expose an application](/{{page.version}}/docs/user-guide/quick-start)
1. [Configuring and launching containers: configuring common container parameters](/{{page.version}}/docs/user-guide/configuring-containers)
1. [Deploying continuously running applications](/{{page.version}}/docs/user-guide/deploying-applications)
1. [Connecting applications: exposing applications to clients and users](/{{page.version}}/docs/user-guide/connecting-applications)
1. [Working with containers in production](/{{page.version}}/docs/user-guide/production-pods)
1. [Managing deployments](/{{page.version}}/docs/user-guide/managing-deployments)
1. [Application introspection and debugging](/{{page.version}}/docs/user-guide/introspection-and-debugging)
    1. [Using the Kubernetes web user interface](/{{page.version}}/docs/user-guide/ui)
    1. [Logging](/{{page.version}}/docs/user-guide/logging)
    1. [Monitoring](/{{page.version}}/docs/user-guide/monitoring)
    1. [Getting into containers via `exec`](/{{page.version}}/docs/user-guide/getting-into-containers)
    1. [Connecting to containers via proxies](/{{page.version}}/docs/user-guide/connecting-to-applications-proxy)
    1. [Connecting to containers via port forwarding](/{{page.version}}/docs/user-guide/connecting-to-applications-port-forward)

## Concept guide

[**Overview**](/{{page.version}}/docs/user-guide/overview)
: A brief overview of Kubernetes concepts.

[**Cluster**](/{{page.version}}/docs/admin/)
: A cluster is a set of physical or virtual machines and other infrastructure resources used by Kubernetes to run your applications.

[**Node**](/{{page.version}}/docs/admin/node)
: A node is a physical or virtual machine running Kubernetes, onto which pods can be scheduled.

[**Pod**](/{{page.version}}/docs/user-guide/pods)
: A pod is a co-located group of containers and volumes.

[**Label**](/{{page.version}}/docs/user-guide/labels)
: A label is a key/value pair that is attached to a resource, such as a pod, to convey a user-defined identifying attribute. Labels can be used to organize and to select subsets of resources.

[**Selector**](/{{page.version}}/docs/user-guide/labels/#label-selectors)
: A selector is an expression that matches labels in order to identify related resources, such as which pods are targeted by a load-balanced service.

[**Replication Controller**](/{{page.version}}/docs/user-guide/replication-controller)
: A replication controller ensures that a specified number of pod replicas are running at any one time. It both allows for easy scaling of replicated systems and handles re-creation of a pod when the machine it is on reboots or otherwise fails.

[**Service**](/{{page.version}}/docs/user-guide/services)
: A service defines a set of pods and a means by which to access them, such as single stable IP address and corresponding DNS name.

[**Volume**](/{{page.version}}/docs/user-guide/volumes)
: A volume is a directory, possibly with some data in it, which is accessible to a Container as part of its filesystem.  Kubernetes volumes build upon [Docker Volumes](https://docs.docker.com/userguide/dockervolumes/), adding provisioning of the volume directory and/or device.

[**Secret**](/{{page.version}}/docs/user-guide/secrets)
: A secret stores sensitive data, such as authentication tokens, which can be made available to containers upon request.

[**Name**](/{{page.version}}/docs/user-guide/identifiers)
: A user- or client-provided name for a resource.

[**Namespace**](/{{page.version}}/docs/user-guide/namespaces)
: A namespace is like a prefix to the name of a resource. Namespaces help different projects, teams, or customers to share a cluster, such as by preventing name collisions between unrelated teams.

[**Annotation**](/{{page.version}}/docs/user-guide/annotations)
: A key/value pair that can hold larger (compared to a label), and possibly not human-readable, data, intended to store non-identifying auxiliary data, especially data manipulated by tools and system extensions.  Efficient filtering by annotation values is not supported.

## Further reading

* API resources
  * [Working with resources](/{{page.version}}/docs/user-guide/working-with-resources)

* Pods and containers
  * [Pod lifecycle and restart policies](/{{page.version}}/docs/user-guide/pod-states)
  * [Lifecycle hooks](/{{page.version}}/docs/user-guide/container-environment)
  * [Compute resources, such as cpu and memory](/{{page.version}}/docs/user-guide/compute-resources)
  * [Specifying commands and requesting capabilities](/{{page.version}}/docs/user-guide/containers)
  * [Downward API: accessing system configuration from a pod](/{{page.version}}/docs/user-guide/downward-api)
  * [Images and registries](/{{page.version}}/docs/user-guide/images)
  * [Migrating from docker-cli to kubectl](/{{page.version}}/docs/user-guide/docker-cli-to-kubectl)
  * [Tips and tricks when working with config](/{{page.version}}/docs/user-guide/config-best-practices)
  * [Assign pods to selected nodes](/{{page.version}}/docs/user-guide/node-selection/)
  * [Perform a rolling update on a running group of pods](/{{page.version}}/docs/user-guide/update-demo/)