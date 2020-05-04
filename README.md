# Linting Dockerfile

---

## Introduction

- Useful [pre-commit](http://pre-commit.com) hooks for checking Dockerfiles for issues.
- Does not require to have `node` or `dockerfilelint` installed: `pre-commit` will fetch and install them under the hood.
- The test `Dockerfile` in this repo was taken from [here](https://github.com/docker-library/redis/blob/master/3.2/Dockerfile).

## Usage

```
- repo: https://github.com/viperactual/viper-dockerfilelint
  rev: v0.1.0
  hooks:
  - id: dockerfilelint
    stages: [commit]
```

## Resources

- Uses https://github.com/replicatedhq/dockerfilelint to lint your Dockerfile
