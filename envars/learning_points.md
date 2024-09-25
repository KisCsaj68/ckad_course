## At lecture
- add `env:` part to the yaml file
- plain key - value
- ConfigMap
- Secrets

### ConfigMap
- key value pair of config data
- store the variables in a central location
- create configMap with imperative , declerative way
- upload the pairs from file
- use full env in pod definition.yaml
- use only single env in pod definition.yaml
- use volume in pod definition.yaml

#### Labs:
- create configmap
- attach to pod
- change envvars in pods

### Secrets
- not store data in plan text
- encodid format base 64
- create secret
- convert plain text to base 65 `echo -n text | base64`
- get the secret values `k get secret [name] -o yaml`
- decode the secret value `k get secret [name] -o jsonpath='{.data.[key]}' | base64 -d` 
- add to pod defination yaml `envFrom: - secretRef: name:[secretName]`
- attach as volume, it is good practice if the secret or configmap data can change during the pod life `volumes: - `

#### Labs:
- create secrets
- use base64 encode / decode
- attach secrets to pod
