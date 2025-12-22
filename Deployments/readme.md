Imperative cmds:
Deployment:

Ex: k create deploy redis -n ckad-ns --image=redis --replicas=3 

To expose a deployment via a service:

k expose deploy <deploy_name> --port=80 --target-port=80 --type=ClusterIp/NodePort --name <service_name> 