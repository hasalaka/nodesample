# nodesample

https://www.tutorialspoint.com/nodejs/nodejs_express_framework.htm



docker tag nodesample:v1 gcr.io/gcp-wow-rwds-hwaravita-poc-dev/nodesample:v1
docker push gcr.io/gcp-wow-rwds-hwaravita-poc-dev/nodesample:v1


#Verify
gcloud container images list
gcloud container images list-tags gcr.io/gcp-wow-rwds-hwaravita-poc-dev/nodesample