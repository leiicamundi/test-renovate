
ARG BASE_IMAGE_NAME="docker.io/bitnami/keycloak:25.0.5-debian-12-r0"

# List of all available images with associated sha: https://hub.docker.com/r/bitnami/keycloak/tags

# Note: use the global image digest to make this image platform agnostic (see: https://github.com/camunda/zeebe/pull/14186)


# We use the identity image to copy the keycloak theme

FROM docker.io/camunda/identity:latest@sha256:c34f3d375dd2b4bf9345b5ca1b5b23dd26af4b07ee77bc4f64918e59fbeeef0e AS identity

FROM ${BASE_IMAGE_NAME} AS builder