# Redpanda-connect-file-demo

Loading a CSV file to AVRO via Redpanda-connect into a Kafka Stream

Development is using Visual Studio Code with the Devcontainer plugin. Once the code is cloned reopen using devcontainers and then run:

```zsh
setup-devcontainer.sh
```

If you would like to include the devcontainers python data tools as well before running setup-devcontainer.sh set the environment variable DATA to true.

## Demo Environment Setup

Setup the demo environment

```zsh
 task demo-start
```

To stop and clean up the demo environment

```zsh
task demo-stop
```
