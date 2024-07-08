# Incremental build

This build depends on a previous Morpheus image. The Tekton Pipeline defaults to the ImageStreamTag
`morpheus:latest` but you can override the `MORPHEUS_CONTAINER` and `MORPHEUS_CONTAINER_TAG` properties
to use a different base image.

The pipeline will use the [Dockerfile](../experimental/event-driven-rag-cve-analysis/Dockerfile) in the Event Driven RAG CVE analysis experimental example to build a Container Image that serves Jupyter Lab through an endpoint.