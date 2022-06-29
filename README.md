## AnujAroshA/hello-go

This is a basic Helm chart to understand and teach the connection of following components

1. Go lang web server
2. Containerized above service in to a [Docker image](https://hub.docker.com/r/anujarosha/hello-go)
3. Packaged that containerized image as a Helm chart

[![Artifact Hub](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/hello-go)](https://artifacthub.io/packages/search?repo=hello-go)

### How to use

```markdown
helm repo add hello-go https://anujarosha.github.io/hello-go/helm/charts
helm repo update
helm repo list
```

### How to bump a version

- Assume you are referring new docker image version, and then you will update the `image.`tag` property in the values.yaml.
- Then you can update `appVersion` accordingly and depend on this is a bug fix of a feature, you can update the `version` property in the Chart.yaml.
- Go inside the _artifacts_ directory create a new helm package
```commandline
helm package ../helm 
```
- Now create the index file for the packages
```commandline
helm repo index .
```
- Add, commit and push your changes to repository.
- If you have already made the link with Git repo and the Artifact Hub, it will take nearly 30 minutes to pop your newly package in the hub.
