#Create Postgres config maps resource
    kubectl create -f postgres-configmap.yaml 
#Create storage related deployments
    kubectl create -f postgres-storage.yaml
#Create Postgres deployment
    kubectl create -f postgres-deployment.yaml 
#Create Postgres Service
    kubectl create -f postgres-service.yaml
#Connect to postgres
    kubectl get svc postgres
#Use port 31070 to connect to PSQL
    psql -h localhost -U postgresadmin1 --password -p 31070 postgresdb




