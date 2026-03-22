🚀 DevOps Project – ArgoCD Kubernetes Deployment

This repository contains Kubernetes manifests used to deploy a full-stack application using ArgoCD (GitOps approach).


Files Overview

🔹 web.yaml

* Deploys the main web application
* Creates a Service to expose the app


🔹 web-ingress.yaml

* Configures Ingress (NGINX)
* Provides external access to the web application via domain/URL



🔹 mongodb-statefulset.yaml

* Deploys MongoDB database using StatefulSet
* Ensures data persistence using Persistent Volumes



🔹 mongodb-secret.yaml

* Stores database credentials
* Used securely by MongoDB and other services



🔹 mongo-configmap.yaml

* Stores non-sensitive configuration
    Example: MongoDB connection URL 



🔹 mongo-express.yaml

* Deploys Mongo Express UI
* Allows you to manage MongoDB from browser


🔹 ksm.yaml

* Deploys kube-state-metrics
* Used for monitoring Kubernetes cluster metrics



🔹 sc.yaml

* Defines StorageClass
* Used for dynamic storage provisioning in Kubernetes

---

How It Works

1. Code is pushed to GitHub
2. ArgoCD watches this repository
3. Automatically applies Kubernetes manifests
4. Application gets deployed to the cluster



This repo shows:

* Kubernetes deployments (web + database)
* GitOps using ArgoCD
* Use of ConfigMap, Secret, StatefulSet, Ingress
* Basic monitoring setup
