
ARG BASE_IMAGE_NAME="docker.io/camunda/keycloak:25.0.5"

# List of all available images with associated sha: https://hub.docker.com/r/bitnami/keycloak/tags

# Note: use the global image digest to make this image platform agnostic (see: https://github.com/camunda/zeebe/pull/14186)


# We use the identity image to copy the keycloak theme

FROM docker.io/camunda/identity:latest@sha256:74f0166a87d1630a1d98815cdfafb6aaebbcea7a296bb99f3ca00d096796200e AS identity

FROM ${BASE_IMAGE_NAME} AS builder