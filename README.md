## NuclearFlux

Reactive observability library for real-time visualization of Spring WebFlux pipelines in Java applications.

The library captures Reactor operators at runtime and renders the execution of reactive pipelines as an interactive visualization in a monitoring server.

## How It Works

1. A method is annotated with `@ObserveFlux`.
2. When the method is invoked, the library intercepts the returned Reactor Publisher (`Flux` or `Mono`).
3. Monitoring hooks are attached to the reactive pipeline.
4. Execution events from each operator are streamed to the observability server.
5. The server renders the pipeline as a real-time interactive visualization.

## Diagram

<Project C4 or sequencial diagram>
  
## Tech Stack

Backend:
- Java 21
- Spring Boot 4.0.0
- Reactor
- WebSocket streaming

Visualization:
- JavaScript
- WebSocket
- Graph rendering

## Use Cases

### @ObserveFlux

Marks a method returning a Reactor Publisher (`Flux` or `Mono`).

When invoked, the library attaches monitoring hooks to the reactive pipeline and streams execution events to the observability server.

Parameters:

- `name` – identifier used in the visualization server.
- If omitted, the method name is used.

If the annotated method does not return a reactive Publisher, the library logs a configuration warning.


```bash
git clone <Link>
cd <Project name>
<other commands>
```

Access:

    <Api routes or swagger>

## Contact
[LinkedIn](https://www.linkedin.com/in/gabriel-gerhardt-0a8b852b9/)

[Gmail](mailto:gabrielgerhardt27@gmail.com)

[GitHub](https://github.com/Gabriel-Gerhardt)

