
ARG BASE_IMAGE_NAME="docker.io/camunda/keycloak:25.0.5-debian-12-r0"

# List of all available images with associated sha: https://hub.docker.com/r/bitnami/keycloak/tags

# Note: use the global image digest to make this image platform agnostic (see: https://github.com/camunda/zeebe/pull/14186)


ARG BASE_IMAGE_DIGEST="sha256:9f38f0d7f1e6ac356684da0ede6d9fa07f19a86270e5baa49afb31b2fdede876"



# We use the identity image to copy the keycloak theme

FROM docker.io/camunda/identity:latest@sha256:c63263df40ee3e7db9e989efc5ebb96010651566d6d4399c0385329b6d0102a3 AS identity

FROM ${BASE_IMAGE_NAME}@${BASE_IMAGE_DIGEST} AS builder