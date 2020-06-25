# cxp-hello-k8s

Simplest possible cloud native java application based on Spring Boot.

As demonstrated in training session.

## Schematics

## HOW-TO create Kubernetes manifests

The templates for the Kubernetes manifests are stored in `src/main/kubernetes/cxp-hello-k8s`.
To resolve all placeholders in these templates, you have to run maven from the project root folder:

```
mvn process-resources -Dk8s.cluster.namespace=miket92 -f pom.xml
```

The final Kubernetes manifests will be copied to `target/kubernetes-resources/cxp-hello-k8s`.

