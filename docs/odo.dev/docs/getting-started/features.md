---
title: Features
sidebar_position: 1
---

# Features provided by odo

odo has a simple "create and push" workflow for almost everything. It means, as a user, when you "create" something the information (or manifest) is stored in a configuration file, and then upon doing a "push" it gets created  on the Kubernetes cluster.

It is very straightforward to take an existing git repository and create an odo component from it which can be pushed to a Kubernetes cluster.

odo helps deploy and link multiple components and services with each other. This in turn makes it a tool to develop and deploy applications following the microservices pattern without having to learn a thing about Kubernetes. 

### What can odo do?

Full details of what each odo command is capable of doing can be found in the "Command Reference" section. Below is a summary of most important capabilities:
* Create a manifest to deploy applications on Kubernetes cluster. odo easily creates a manifest for existing projects as well as new ones.
* Securely expose the application running on Kubernetes cluster to access it from developer's machine.
* Easily add storage to the application.
* Create and link to services created from [Kubernetes Operators](https://github.com/operator-framework/).
* Link among multiple applications (microservices) deployed as odo components.
* Debug a remote application on your IDE.
* Run tests on the application deployed on Kubernetes.

### What can odo not do?

As discussed in [Introduction](../intro.md), odo is not meant for ops centric users and hence it cannot be used to manage a Kubernetes cluster. It is also not recommended to use odo to deploy applications to production Kubernetes cluster yet.

### What will odo never do?

odo will never try to do things that `kubectl` and `oc` are already good at. Having said that, odo is continuously looking for ideas and ways to abstract Kubernetes features to make them easily consumable by applicatoin developers. If you have any feature requests, please open an issue on [our GitHub repository](https://github.com/openshift/odo/).

### What features to expect in odo?

We are working on some exciting features like:
* Linking to services created using Helm package manager.
* Create `odo deploy` command to transition from inner loop to outer loop.
* Support for Knative eventing.

For a quick high level summary of the features we're planning to add, take a look at [odo milestones](https://github.com/openshift/odo/milestones).