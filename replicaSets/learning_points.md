## At practice test:
- check running ReplicaSet
- delete pods and ReplicaSet ensure that exact number of pods running
- find mistakes in definition.yaml files
- find why pods are down
- redirect a running ReplicaSEt properties into yaml (k get rs `ReplicaSet name` -o yaml > ra-def.yaml)
- scale up replicas
- scale down replicas


## Lecture
- Difference between ReplicationController and ReplicaSet
- importance of lables and Selectors
- Create basic yaml to create ReplicaSet
- Scale up the ReplicaSet
  - in the yaml file and replace  - f to replace the old one
  - k scale --replicas=6 -f rs-def.yml
  - k scale --replicas=6 replicaset myapp-replicaset