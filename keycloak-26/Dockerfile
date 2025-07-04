
ARG BASE_IMAGE_NAME="docker.io/bitnami/keycloak:26.3.0-debian-12-r0"

# List of all available images with associated sha: https://hub.docker.com/r/bitnami/keycloak/tags

# Note: use the global image digest to make this image platform agnostic (see: https://github.com/camunda/zeebe/pull/14186)


ARG BASE_IMAGE_DIGEST="sha256:f5727c6357f947beda242391a9c6add244b50d5b179687e6c6d1a919f9f5293e"



# We use the identity image to copy the keycloak theme

FROM docker.io/camunda/identity:latest@sha256:74f0166a87d1630a1d98815cdfafb6aaebbcea7a296bb99f3ca00d096796200e AS identity

FROM ${BASE_IMAGE_NAME}@${BASE_IMAGE_DIGEST} AS builder