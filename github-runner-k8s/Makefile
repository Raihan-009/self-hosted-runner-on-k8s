build:
	docker build -t poridhi/our-runner:v1.1 .

push:
	docker push poridhi/our-runner:v1.1

namespace:
	kubectl create ns host-runner

secrets:
	kubectl -n host-runner create secret generic github-secret \
			--from-literal=GITHUB_OWNER=Raihan-009 \
			--from-literal=GITHUB_REPOSITORY=self-hosted-runner-on-k8s \
			--from-literal=GITHUB_PERSONAL_TOKEN=""


