# k8sdashboard-helm
Helm Chart for installing k8s dashboard in read only mode. 

# Features
This chart has been tested in AWS.
It uses metrics-server.
The ROLES used make sure that it can't be used for updating anything in the cluster.
This should ideally be put behind a firewall and/or with access restricted to your corporate/personal network CIDR. This can be achieved providing appropriate values in the included values.yaml file which controls creation of an alb-ingress in AWS.
