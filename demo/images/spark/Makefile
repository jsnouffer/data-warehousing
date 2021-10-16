# HELP
.PHONY: help

image = pyspark
tag = 3.1.2

help: ## This help.
	@awk 'BEGIN {FS = ":.*?## "} /^[a-zA-Z_-]+:.*?## / {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}' $(MAKEFILE_LIST)

build: ## Build container image
	docker build -t $(image):${tag} --build-arg SPARK_VERSION=${tag} .

run: ## Run container image
	docker run -it --rm --name="${image}" $(image):${tag}

