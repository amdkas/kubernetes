IMAGE_NAME ?= yannig/eni-flask-healthcheck
VERSION    ?= $(shell git rev-parse --abbrev-ref HEAD)

build:
	docker build -t $(IMAGE_NAME):$(VERSION) .

run-test:
	docker run -it --rm --network host $(IMAGE_NAME):$(VERSION)
