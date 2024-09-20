## At practice test:
- find namespaces
- find pod @namespace
- call service at same ns
- call service at different ns

## At lecture:
- automatically created ns:
 - kube-system
 - default
 - kube-public
- how to reach ns: `.dev.svc.cluster.local`
- command use --namespace= flag
- add ns data to pod-definiton file
- create ns with `.yaml`
- k create ns dev
- config context to a fix ns `k config set-context $(kubectl config current-context) --namespace=dev` or `kubens`
- to see pods all ns -A
- set up resource quote for ns