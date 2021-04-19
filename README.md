What I want to show:

- How to setup a local k8s cluster
- How to configure a set of nodes and make sure that they are configured in the same way
- How to build a few microservices which implement the Saga Orch pattern
- How to host a discovery service (istio.io)
- How to use keptn
- How to monitor the setup

# microcloud

This is a small but hands on example about how to build your own k8s cluster and run a Saga micro service on those nodes

# Pre-requesits

- VirtualBox
- Multipass

# Steps

## Preparation

Install the tools mentioned in the Pre-requesits section and create 4 Linux Machines locally. These machines will serve as your environment for your k8s cluster

```
multipass launch --name linux1
multipass launch --name linux2
multipass launch --name linux3
multipass launch --name linux4
```

The first command takes a while as the images needs to get downloaded.

Verify the startup of the machines with `multipass list`. This should give you the following:
