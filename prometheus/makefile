validate:
	kubectl create namespace monitoring
	kubectl create -f ./config-map.yaml --namespace monitoring
install: validate
	kubectl create -f ./prometheus-deployment.yaml --namespace monitoring
service:
	kubectl create -f ./prometheus-service.yaml
status:
	kubectl get configmap
	kubectl get deployment
	kubectl get service 
