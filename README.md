
## About The Assignment : 
Create Kubernetes config to launch Clickhouse & Superset pods in Minikube & connect them.

## Quick Usage :
We will run the project locally :
  - Clone the repo : ```git clone [repo-url]```
  - Start minikube : ```minikube start --driver=docker```
  - Run .yaml files : ``` kubectl apply -f <file-name>.yaml```
  - Run command to create a service that exposes a Kubernetes deployment to external traffic : ```kubectl expose deployment superset --type=NodePort --port=8088```
  - Check all the running pods ```kubectl get pods```
  - Check all the services ```kubectl get services```. After you will be assgined a Cluster IP adresss and Port of clickhouse. for example IP: ```10.97.156.250``` PORT: `8123`.
  - Use the IP Address to access the superset services.
  - Username : ```admin``` Password : ```admin```
  - To Connect clickhouse to superset.
  -- Go to ```Data > Databases > + Database```. Select Clickhouse database.
-- Cofigure the with clickhouse IP: `10.97.156.250` address and PORT `8123`.
--You will be Clickhouse & Superset pods in Minikube.
