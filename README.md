# Quarkus NPE in dev-mode

This project aims to demonstrate a NullPointerException bug that happens in dev mode when a ["source" is missing in 
the recompilation diagnostics]()

This project was generated using the [quarkus maven plugin](https://quarkus.io/guides/getting-started-guide).

It simply adds the tinkerpop gremlin core maven dependency :
```
    <dependency>
      <groupId>org.apache.tinkerpop</groupId>
      <artifactId>gremlin-core</artifactId>
      <version>3.3.3</version>
    </dependency>
```

## Usage

Start the project using this command :
```
mvn clean compile quarkus:dev
```

Open your browser at http://127.0.0.1:8080/

Edit any source file, save it, then refresh the page in your browser: **the error will be displayed**.