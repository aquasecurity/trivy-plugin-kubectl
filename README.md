# trivy-plugin-docker
A [Trivy](https://github.com/aquasecurity/trivy) plugin that scans the images of a kubernetes resource

## Install

```
$ trivy plugin install github.com/aquasecurity/trivy-plugin-docker
$ trivy docker -h
Usage: trivy docker [-h,--help] TYPE NAME [TRIVY OPTION]
 A Trivy plugin that scans the images of a kubernetes resource.

Options:
  -h, --help    Show usage.

Examples:
  # Scan docker images
  trivy docker 

  # Scan docker images and filter by severity
  trivy docker  -- --severity CRITICAL
```

## Usage
Trivy's options need to be passed after `--`.

```
  # Scan docker images
  trivy docker 

  # Scan docker images and filter by severity
  trivy docker  -- --severity CRITICAL
```

