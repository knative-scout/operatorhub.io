.PHONY: docker-build docker-run docker-push

DOCKER_TAG_VERSION ?= dev-latest
DOCKER_TAG ?= docker.io/kscout/site:${DOCKER_TAG_VERSION}

docker-build:
	docker build -t ${DOCKER_TAG} .

docker-run:
	docker run \
		-it --rm --net host \
		${DOCKER_TAG}

docker-push:
	docker push ${DOCKER_TAG}
