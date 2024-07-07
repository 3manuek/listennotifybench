# listennotifybench

Postgres' Listen/Notify Benchmark. 

## Abstract 

Listen/Notify feature is an old Postgres' feature that allows to use the database
instance as a Message Broker. 

I have a previous work on this at [listen_notify_bench](https://github.com/3manuek/listen_notify_bench),
but it's quite old and is not exactly for this project.

## Phases

- Build an enviroment to test the patch and vanilla.
- Build the client, and measure the throughput, reproducing what has 
  been done in the original post.
