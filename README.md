# Pipeline e repositório de imagens compartilhado

- Git: `https://github.com/raphac-mar/01-pipelines`

## k8s

1. Criar namespace para pipelines compartilhado

- pipelines-ns.yaml

2. Criar PVC para pipelines

- pipelines-shared-workspace-pvc.yaml

3. Criar namespace para repositório de imagens compartilhado

- pipelines-ir-ns.yaml

4. Criar permissão para pipeline, de image builder, no repositório de imagens compartilhado

- pipelines-ir-rbac-pipeline-image-builder.yaml

## Argo CD

```sh
cd 01-pipelines
oc apply -f argocd/application.yaml
```
