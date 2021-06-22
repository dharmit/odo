---
sidebar_position: 1
title: Introduction
---

### What is odo?

odo is a command line tool that helps develop and deploy applications to a Kubernetes cluster. It abstracts the Kubernetes terminology so that an application developer can focus on writing code in their favourite framework without having to learn a thing about Kubernetes.

odo is focussed on inner loop development with some tooling that would help users transition to the outer loop. 

Brendan Burns, the cofounder of Kubernetes, said in the [book Kubernetes Patterns](https://www.redhat.com/cms/managed-files/cm-oreilly-kubernetes-patterns-ebook-f19824-201910-en.pdf):

> It (Kubernetes) is the foundation on which applications will be built, and it provides a large library of APIs and tools for building these applications, but it does little to provide the application architect or developer with any hints or guidance for how these various pieces can be combined into a complete, reliable system that satisfies their business needs and goals.

It is the application architects and developers that odo aims to make Kubernetes easy for.

### What is "inner loop"?

In simplest terms, inner loop is the phase before the developer does `git commit`. odo workflow helps the developers take a look at how their application will behave when deployed to a Kubernetes cluster.   

### Who should use odo?

You should use odo if:
* you are developing applications using Node.js, Spring Boot, or similar framework
* your applications are deployed on Kubernetes
* you don't want to spend time learning about Kubernetes, but want to develop applications using your favourite framework

Basically, if you are an application developer, you should use odo to deploy your application on a Kubernetes cluster.

### Who should _not_ use odo?

You should not use odo if:
* you maintain a production Kubernetes cluster
* you have to perform administration tasks against a Kubernetes cluster

Basically, if you are an ops person, odo is not the tool for you.

### How is odo different from `kubectl` and `oc`?

odo is different from [`kubectl`](https://github.com/kubernetes/kubectl) and [`oc`](https://github.com/openshift/oc/) in that it is focussed on developers. Both `kubectl` and `oc` are ops focussed tools and help in deploying applications to and maintaining a Kubernetes cluster.