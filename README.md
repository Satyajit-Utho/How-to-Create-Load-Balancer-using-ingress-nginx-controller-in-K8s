# How-to-Create-Load-Balancer-using-ingress-nginx-controller-in-K8s
Load Balancer using ingress-nginx-controller in K8s

# Setting Up a Load Balancer with Ingress-NGINX-Controller in Utho Cloud Kubernetes

This guide walks you through the steps to set up a Load Balancer in a Kubernetes (K8s) cluster using the `ingress-nginx-controller` in Utho Cloud. It will help you route HTTP/S traffic to services and provide a scalable, robust solution for managing incoming requests.

## Prerequisites

Before proceeding, ensure you have the following:

- A running Kubernetes cluster on **Utho Cloud**.
- **kubectl** installed and configured to interact with your Utho Cloud K8s cluster.
- **Helm 3+** installed for easy deployment (optional but recommended).

## Steps to Set Up a Load Balancer with Ingress-NGINX-Controller

### Step 1: Install Ingress-NGINX Using Helm

The easiest way to install the NGINX ingress controller is using Helm.

1. Add the NGINX ingress controller Helm chart:

```bash
# Add the NGINX ingress controller repository to Helm
helm repo add ingress-nginx https://kubernetes.github.io/ingress-nginx

# Update the Helm repositories to get the latest charts
helm repo update
