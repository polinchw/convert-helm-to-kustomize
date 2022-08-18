# Convert Helm Chart to Kustomize

## Steps to convert a helm chart to Kustomize app

```
helm template bitnami/tomcat --output-dir .

cd tomcat/

mv templates/ base/

kustomize create --autodetect

```