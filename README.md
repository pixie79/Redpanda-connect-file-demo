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

To load the file into s3 and trigger the bucket notification

```zsh
task demo-cp
```

To stop and clean up the demo environment

```zsh
task demo-stop
```

When the demo is running you can do *task logs* to see the docker logs for the connect container. Please do ignore the first 30 seconds of log (hence the sleep in the startup)
as this is while the containers settle down and the bucket / sqs queue is being setup.
