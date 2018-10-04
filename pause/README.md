# Toy deployment

Install:

    kustomize build | kubectl -n playground apply -f - -lapp.kubernetes.io/instance=pause-playground-01 --dry-run

Remove:

    kustomize build | kubectl -n playground delete -f - --dry-run
