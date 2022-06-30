## AnujAroshA/hello-go

This is a basic Helm chart to understand and teach the connection of following components

1. Go lang web server
2. Containerized above service in to a [Docker image](https://hub.docker.com/r/anujarosha/hello-go)
3. Packaged that containerized image as a Helm chart

### How to use

```markdown
# Can confirm repo is added
helm repo list

# Update the repo if you have already added it
helm repo update
```

As per now, only endpoints that you can check are `/hi` and `/hello`

Ex. http://localhost:8081/hi
