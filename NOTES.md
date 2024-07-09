# Notes

## Links

- [listen_notify_bench](https://github.com/3manuek/listen_notify_bench)

Related to runtime debugging:

- [runtime config developer](https://www.postgresql.org/docs/devel/runtime-config-developer.html), see `trace_notify`. [trace_notify GUC](https://www.postgresql.org/docs/devel/runtime-config-developer.html#GUC-TRACE-NOTIFY).
- Implement [devcontainers](https://github.com/atomicdb/devcontainer/tree/main) but for runtime debugging.


Relevant:

- [Support wildcards in LISTEN NOTIFY](https://commitfest.postgresql.org/48/4896/)
  - Implements [Digital BinaryTrie](https://www.opendatastructures.org/ods-java/13_1_BinaryTrie_digital_sea.html)
  - [Thread](https://www.postgresql.org/message-id/flat/CAN_hQmuysJpMzWcyhQwYtHpao8XXMpc48A8F=n-0e6x_z2P_Fw@mail.gmail.com)

Links to related projects that worth a reading about the matter:

- [pglistener](https://gitlab.com/microo8/pglistener/-/tree/master?ref_type=heads)
- [Postgres Listen/Notify](https://tapoueh.org/blog/2018/07/postgresql-listen/notify/)
- [libpq example docs](https://www.postgresql.org/docs/16/libpq-example.html)


Application side approaches:

- [Message Broker in Java](https://www.baeldung.com/spring-postgresql-message-broker)
- [pg-ipc](https://github.com/emilbayes/pg-ipc/tree/master)
- [Spring Listen Notify](https://dzone.com/articles/leveraging-postgres-listennotify-in-spring-boot)
- [](https://gitlab.com/3manuek/benchmark)

## Building a container environment

- Using Earthly will provide some abstraction of the container build. 
- The ability to push the generated patches as functional images
- The ability to set a debug flag through the process, when `--interactive` is set. 
- https://github.com/atomicdb/devcontainer/tree/main/postgres integrate with devcontainers

## Ideas for the benchmark model


### Case Alerting 

```mermaid

```

<DOMAIN>.ALERTS.ANOMALY
<DOMAIN>.ALERTS.ABUSE
<DOMAIN>.INFORMATION.STATUS

