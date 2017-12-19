validate:
	kubectl create namespace monitoring
	kubectl create -f ./config-map.yaml --namespace monitoring
install: validate
	kubectl create -f ./prometheus-deployment.yaml --namespace monitoring
service:
	kubectl create -f ./prometheus-service.yaml --namespace monitoring
status:
	kubectl get configmap --namespace monitoring
	kubectl get deployment --namespace monitoring
	kubectl get service --namespace monitoring 
