# Kubernetes "Demo": Improving App Secrets Config and Adding an Ingress

## Goals

* Recap & complete the namespace deployment for dev, qa, and prod todoapi environments, using the [Aug 13 writeup](https://github.com/us-learn-and-devops/2021_08_13) as reference (part 6)
* Secrets update:
  * Use a volume mount to consume the DB secrets
  * Use a docker-registry/image-pull `secret` to deploy `todoapi` via a private Docker registry
  * Ensure we're also creating our existing DB `secret`s securely
* Ingress:
  * Recap our options for configuring access to our deployed pods
  * Briefly discuss ingress controller/resource (in relation to service resources/types)
  * Install an ingress controller and ingress resource
  * Deploy a 2nd "echo" service to our k8s cluster
  * Update the ingress to give access to both backend serices
* (Time allowing) Briefly discuss concepts used in or related to material from today...
  * volumes & volume mounts
  * cloud volumes
  * stateful sets

## Lab

### 1. Setup

Check out [the 1.2.0 release](https://github.com/us-learn-and-devops/todoapi/releases/tag/1.2.0) of the `todoapi` repo in us-learn-and-devops GitHub.

Run the `/build/cluster-deploy.sh` script (or equivalent) to get your k8s cluster up and running.

### 2. Demo

...
