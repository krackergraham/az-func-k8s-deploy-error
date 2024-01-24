## Repro Steps

1. `func init --docker --worker-runtime node --language typescript`

2. `func new --name httpTrigger --template "HTTP trigger" --authlevel "anonymous"`
3. `func kubernetes deploy --name myfunc --service-type ClusterIP --namespace <keda_namespace> --debug --registry <local_registry> --write-configs`
4. See config in `functions.yaml`
