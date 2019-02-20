# Purpose
Sample of running PingDirectory on GKE. 

## Contents: 
* [Prerequisites](prerequisites)
* [Setup](Setup)
* [Deploy](deploy)

## Prerequisites
* Google Cloud Platform account with active billing
* `kubectl` and `gloucd` command line tools
* an active project with billing and APIs turned on and an active cluster
> If you need help with any of these steps, please refer to the corresponding steps from [try-gke](https://github.com/GoogleCloudPlatform/kubernetes-engine-samples/blob/master/try-gke/README.md)



##Setup
tbd

## Deploy
1. Open a terminal and cd to this directory

2. You will need a Persistent volume claim:
`kubectl apply -f pd-volumeclaim.yaml`

3. deploy: 
`kubectl create -f ping_directory.yaml`

4. view logs:
`kubectl logs -lapp=pingdirectory`