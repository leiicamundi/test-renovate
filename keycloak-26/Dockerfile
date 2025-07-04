
ARG BASE_IMAGE_NAME="docker.io/bitnami/keycloak:26.2.5-debian-12-r2"

# List of all available images with associated sha: https://hub.docker.com/r/bitnami/keycloak/tags

# Note: use the global image digest to make this image platform agnostic (see: https://github.com/camunda/zeebe/pull/14186)


ARG BASE_IMAGE_DIGEST="sha256:e623429e6967f2080122a1d491394d20adf7a913bf12aea45c7b48617946f394"



# We use the identity image to copy the keycloak theme

FROM docker.io/camunda/identity:latest@sha256:c63263df40ee3e7db9e989efc5ebb96010651566d6d4399c0385329b6d0102a3 AS identity

FROM ${BASE_IMAGE_NAME}@${BASE_IMAGE_DIGEST} AS builder