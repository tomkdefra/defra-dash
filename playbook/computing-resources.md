---
layout: default
title: Computing Resources
parent: Platform Components
grand_parent: Playbook
nav_order: 1
---

# Computing Resources

## What are clusters?

To be able to run code on the DASH platform, you need to access computational resource to run your code. In Databricks, computing resources are called clusters. A Databricks cluster is a set of computational resources and configurations on which you run data engineering, data science and data analytics workloads, from producing summary statistics and visualisations all the way through to machine learning and complex geospatial analysis.

By default, some of the clusters are always on, whilst others need to be turned on for users to be able to use them. Some users have the right to turn clusters on themselves, they are called business admin users. You can request business admin rights if you would like to be able to turn clusters on. This is particularly relevant if you want to use the notebook cluster or the geospatial clusters.

These clusters can be tailored to a specific task. For example, clusters will have a defined array of packages and libraries pre-loaded at start-up. Users are free to install libraries or packages, but these will not persist after the cluster has been restarted. DASH Platform users are not currently able to develop cluster configurations in the shared workspace, although a series of pre-built configurations have been developed. By default, users will have access to all the below clusters for their work.

## Preconfigured clusters in the shared Databricks Workspace

### RStudio clusters

These are general use clusters that users will do most of their basic analytics on. They are the only clusters that have RStudio as an app, and so all users looking to use RStudio will use these cluster.

The clusters are called: 

- 1a_RStudio
- 1b_RStudio

To check which R version and which packages (including versions) are pre-installed on the RStudio clusters, you need to check which Databricks runtime is used and then check this against the Databricks documentation. For example, a cluster with runtime 13.3 ML will have R version 4.2.2 and the following packages pre-installed: Databricks Runtime 13.3 ML. Please note that if one is creating their own Personal Compute cluster they will need to use an ML Databricks runtime and have auto-termination disabled.