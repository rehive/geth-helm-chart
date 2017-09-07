# geth-helm-chart

1. Create a disk on google cloud:
	`gcloud compute disks create geth-data-testnet --zone europe-west1-c --size 200 --type pd-standard`

2. Fill in the values in `staging/values.yaml`

3. Install the Helm chart:
	`helm install --name geth-testnet --namespace ethereum-service-testnet -f ./staging/values.yaml ./geth-chart/`