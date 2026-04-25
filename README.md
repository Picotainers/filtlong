# filtlong

[Filtlong](https://github.com/rrwick/Filtlong) filters long-read sequencing data by quality and length, helping keep the best reads for assembly and downstream analysis.

## Quick Usage

```bash
docker run --rm docker.io/picotainers/filtlong filtlong --help
```

## Usage

```bash
# Show help
docker run --rm docker.io/picotainers/filtlong filtlong --help

# Filter reads and write output to your local folder
docker run --rm -v "$(pwd):/data" docker.io/picotainers/filtlong \
  filtlong --min_length 1000 /data/reads.fastq > filtered.fastq
```

## Building

```bash
docker build -t picotainers/filtlong .
```
