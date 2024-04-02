---
layout: default
title: Data
parent: Platform Components
grand_parent: Playbook
nav_order: 2
---

# Data

## DASH Data Lake

### Use case

The use case for the Data Lake is to provide a storage environment for data items which are:
  
-   Over 2 GB file size  (We hold smaller datasets than this, the 2GB only relates to the max size that users can load data themselves)

-   Covered by security or licencing constraints (We hold open datasets as well)

-   Likely to be widely useful across Defra group

The Data Lake also allows for automated pipelines to update data at regular intervals and provide pre-processing if required. This data can be of any size or format, although there are formats that are better suited for use on the DASH Platform (see section \@ref(parquet)).

Data stored in the base zone of the Data Lake (see \@ref(data-lake-zones)) is linked to the DASH data catalogue and will enable the sharing of data with other DASH Platform users.