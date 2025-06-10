# Main Docker Compose project
This is a project that is intended to serve as a global system wise solution to 
develop on your machine. By default for now it uses traefik as a main entrypoint to
your application. All the other projects that you will develop, will use this traefik 
route gateway and with help of `/etc/hosts` file in order to not remember ports etc.

## How to run?
Simple, just run
```
docker compose up
```
And then every underlying project will be able to use the traefik installation 
and just add a line in your `/etc/hosts` file with the address and you're good to go!  

## Planned features

- Add Prometheus, Grafana etc in order to have logs in centralized place, similar 
to Datadog or Sentry.
- Add a production ready setup for VPS-es and physical machines that can be deployed.
