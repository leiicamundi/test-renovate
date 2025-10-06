
ARG BASE_IMAGE_NAME="docker.io/bitnami/keycloak:25.0.5-debian-12-r0"

# List of all available images with associated sha: https://hub.docker.com/r/bitnami/keycloak/tags

# Note: use the global image digest to make this image platform agnostic (see: https://github.com/camunda/zeebe/pull/14186)


# We use the identity image to copy the keycloak theme

FROM docker.io/camunda/identity:latest@sha256:adab0ea207916d94cb1a6b917eca512210a27ab3a00f52c7cff22fff36a4ca9f AS identity

FROM ${BASE_IMAGE_NAME} AS builder