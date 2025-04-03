# Vector Setup

Vector is a powerful tool for building observability pipelines. Specifically we are using it for telementry log filtering, transformation and shipping to Axiom.

## Installation

You're probably going to want to install Vector as a daemon on your Algorand node and manage via a process manager. If so [install using the instructions here](https://vector.dev/docs/administration/management/).

## Configuration

The [vector.yaml](./vector.yaml) configuration file describes the pipeline for retrieving, transforming and publishing the log events.

Before uploading the configuration to your node, you will need to provide the following configuration items:

- Your Axiom token
- Your Axion dataset name

Once you have reviewed and refined the configuration, you can copy the contents of the [vector.yaml](./vector.yaml) configuration file to `/etc/vector/vector.yaml` on your Algorand node.
