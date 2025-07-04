
ARG BASE_IMAGE_NAME="docker.io/bitnami/keycloak:25.0.5-debian-12-r0"

# List of all available images with associated sha: https://hub.docker.com/r/bitnami/keycloak/tags

# Note: use the global image digest to make this image platform agnostic (see: https://github.com/camunda/zeebe/pull/14186)


ARG BASE_IMAGE_DIGEST="sha256:17c14caf6e4be214f3a2f82a51b93fe6c50a12f7ed82837341d9d7b5597bc40a"



# We use the identity image to copy the keycloak theme

FROM docker.io/camunda/identity:latest@sha256:74f0166a87d1630a1d98815cdfafb6aaebbcea7a296bb99f3ca00d096796200e AS identity