## AnujAroshA/hello-go

This is a basic Helm chart to understand and teach the connection of following components

1. Go lang web server
2. Containerized above service in to a [Docker image](https://hub.docker.com/repository/docker/anujarosha/hello-go)
3. Packaged that containerized image as a Helm chart

### How to use

```markdown
helm repo add hello-go https://anujarosha.github.io/hello-go/helm/charts
helm repo update
helm repo list
```