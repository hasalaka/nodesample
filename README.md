# nodesample

https://www.tutorialspoint.com/nodejs/nodejs_express_framework.htm

1)
docker build -t gcr.io/gcp-wow-rwds-hwaravita-poc-dev/nodesample:v2 .
OR
docker tag nodesample:v1 gcr.io/gcp-wow-rwds-hwaravita-poc-dev/nodesample:v1

2) docker push gcr.io/gcp-wow-rwds-hwaravita-poc-dev/nodesample:v1


3) Verify
gcloud container images list
gcloud container images list-tags gcr.io/gcp-wow-rwds-hwaravita-poc-dev/nodesample


#kubectl expose deployment samplenodeapp-deployment --type=NodePort --port=3000 --target-port=30000 --name=sample-node-service 


4) Update deployment
kubectl set image deployment/samplenodeapp-deployment nodeapp=gcr.io/gcp-wow-rwds-hwaravita-poc-dev/nodesample:v1 --record

gke-replication-cluster-da7fe96c-node

http://35.189.36.92:30007