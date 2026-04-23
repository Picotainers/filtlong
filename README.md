# filtlong
Small source-built container for `filtlong`.

## Quick Usage

```bash
# Pull the image
docker pull docker.io/picotainers/filtlong:latest

# Run the tool
docker run --rm docker.io/picotainers/filtlong:latest filtlong --help
```

## Run with mounted local data

```bash
docker run --rm -v "$(pwd):/data" docker.io/picotainers/filtlong:latest filtlong --help
```
