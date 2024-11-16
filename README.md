# Kobornetes for dummies

## What is k8s?

kubernetes is a container orchestration platform to manage containerized application

## Cluster Architecture

A cluster consists of one control plane and at least one worker node.
Worker node is where containerized application running, to be precise inside a pod

Cluster components

- kube api server
- etcd -> key-value storage that store all information about cluster
- scheduler -> listening on cluster event, watching cluster changes and react based on cluster spec
- controller manager

Node components

- kubelet -> an agent that deliver information related to container runtime
- kube-proxy -> handle node networking
- pod -> container application running inside this component
