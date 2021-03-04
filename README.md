# trivy-plugin-kubectl
A [Trivy](https://github.com/aquasecurity/trivy) plugin that scans the images of a kubernetes resource

## Install

```
$ trivy plugin install github.com/aquasecurity/trivy-plugin-kubectl
$ trivy kubectl -h
Usage: trivy kubectl [-h,--help] TYPE NAME [TRIVY OPTION]
 A Trivy plugin that scans the images of a kubernetes resource.

Options:
  -h, --help    Show usage.

Examples:
  # Scan a Pod
  kubectl trivy pod mypod

  # Scan a Deployment
  kubectl trivy deployment mydeployment -n mynamespace

  # Scan a Job and filter by severity
  kubectl trivy job myjob -n mynamespace -- --severity CRITICAL
```

## Usage
Trivy's options need to be passed after `--`.

```
# Scan a Pod
$ kubectl trivy pod mypod

# Scan a Deployment
$ kubectl trivy deployment mydeployment -n mynamespace

# Scan a Job and filter by severity
$ kubectl trivy job myjob -n mynamespace -- --severity CRITICAL
```

