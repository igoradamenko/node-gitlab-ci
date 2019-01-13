# Node.js GitLab CI

Docker image that I use in my GitLab projects to build them on CI.

## Example

Create `.gitlab-ci.yml` in the root of your project like this:

```yaml
image: igoradamenko/node-gitlab-ci:latest
```

Then configure your jobs as described in [the documentation](https://docs.gitlab.com/ee/ci/yaml/).

## Why?

In the past I used to write the commands from [Dockerfile](Dockerfile) in `.gitlab-ci.yml`,
but it slowed down builds, and moving them from the separated image saved me 30-60 seconds on each build.
