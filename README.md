reproducer:

```bash
mvn quarkus:dev
```

open http://localhost:8080/hawtio/camel/contexts
click "suspend"


After suspending, route continues to get executed:

```bash
2024-06-20 07:54:07,252 INFO  [org.apa.cam.imp.eng.AbstractCamelContext] (executor-thread-3) Apache Camel 4.5.0 (behaim-its-kaoto) is suspending
2024-06-20 07:54:07,253 INFO  [org.apa.cam.imp.eng.AbstractCamelContext] (executor-thread-3) Apache Camel 4.5.0 (behaim-its-kaoto) is suspended in 0ms
2024-06-20 07:54:09,631 INFO  [beh.cam.yaml:16] (Camel (camel-1) thread #1 - timer://yaml) Hello Camel from anton-to-behaim-its
2024-06-20 07:54:14,633 INFO  [beh.cam.yaml:16] (Camel (camel-1) thread #1 - timer://yaml) Hello Camel from anton-to-behaim-its
```