# local_deployments
Contains the scripts for deploying to k8s clusters

# Deploying environment secrets
Set the secrets as environment variables and run the deployment using
'envsubst < secrets.yaml | kubectl apply -f -'

# Setting up nginx
On the host machine, nginx will be needed for routing external calls to k8s. This is done by installing nginx and adding the contents of <this_repo>/nginx.conf to the end of /etc/nginx/nginx.conf.
