# Field staff docs on Cloud Native products

> **Information classification:** INTERNAL - This data contains information
> about usual company operations, procedures etc. that should not be shared
> publicly, but are intended to be available for all company personnel. Access
> by third parties must be authorized by manager. Disclosure of this
> information would have little business impact and would lead to a minor
> incident.

## Required Kubernetes skills

> **IMPORTANT:** Proficient Kubernetes knowledge is required to work with
> the operator. The Cloud Native team recommends that engineers study
> to get the "Certified Kubernetes Administration (CKA)" certification
> from CNCF to deliver the best quality service about PostgreSQL on
> Kubernetes.

For building a foundation, SEs and Field CTOs should at least take the ["Kubernetes Essentials"](https://linuxacademy.com/cp/modules/view/id/281)
training on Linux Academy.

The ["Cloud Native Certified Kubernetes Administrator (CKA)"](https://linuxacademy.com/cp/modules/view/id/327)
training from Linux Academy provides a fast track for the basics of Kubernetes administration.
However, the best training experience on Kubernetes, also for CKA certification, is provided by
["Certified Kubernetes Administrator (CKA) with practice tests"](https://www.udemy.com/share/101WmEBksZdlxQQ3o=/)
by [Mumshad Mannanbeth](https://www.udemy.com/user/mumshad-mannambeth/) available on Udemy.

## Demo about Cloud Native PostgreSQL on Kubernetes

Cloud Native PostgreSQL is an operator for Kubernetes that
implements the primary/standby architecture in PostgreSQL.

Use the following outline if you want to prepare a demonstration
of the operator using a local Kubernetes cluster with Kind.

1. [Requirements](cnp/requirements.md): what to do in preparation of the demo
1. [Operator deployment](cnp/operator_deployment.md): how to deploy the operator
1. [PostgreSQL cluster deployment](cnp/cluster_deployment.md): how to deploy a PostgreSQL cluster with a primary and an arbitrary number of replicas in a fully declarative way, using just a YAML file
1. [Immutable Application Container](cnp/immutable_application_container.md): practice with the limitations that immutable application containers introduce when working with PostgreSQL, compared to traditional environments
1. [Connection to the PostgreSQL cluster](cnp/connection_postgresql.md): how to connect to any instance of the PostgreSQL cluster
1. [Overview of built-in TLS capabilities](cnp/tls_capabilities.md): a close look at the native support for TLS connections automatically deployed by the operator, including client certificate authentication
1. [Streaming replication](cnp/streaming_replication.md): overview of the native streaming replication support automatically implemented by the operator, including quorum-based synchronous replication
1. [Monitoring and logging](cnp/observability.md): how to access logs, events and metrics of the PostgreSQL cluster
1. [Simulation of a primary failover](cnp/simulation_primary_failover.md): simulate one of the most dreaded incidents that a PostgreSQL database can experience in its lifetime, a failover, and observe how the operator reacts and self-heals the cluster
1. [PostgreSQL configuration](cnp/postgresql_guc.md): change PostgreSQL GUC settings directly from the `Cluster` configuration, using YAML, and observe how PostgreSQL is automatically reload and restarted when necessary
1. [Rolling Updates](cnp/rolling_updates.md): how to execute a rolling update procedure to perform a PostgreSQL minor version update
1. [EDB Postgres Advanced](cnp/edbpa_evaluation.md) : how to enable EDB Postgres Advanced in the demo using your trial license key or the customer's
1. [Backup](cnp/backup.md): this section is still incomplete

> (please expand with monitoring, alerting, Prometheus, Grafana, backup, recovery, ...)

## Demo about Cloud Native PostgreSQL on OpenShift

TODO
