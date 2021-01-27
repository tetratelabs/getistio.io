---
title: "getistio list"
url: /getistio-cli/reference/getistio_list/
---
## getistio list

List available istio distributions built by Tetrate

#### Synopsis

List available istio distributions built by Tetrate

```
getistio list [flags]
```

#### Examples

```
$ getistio list

ISTIO VERSION	FLAVOR 	FLAVOR VERSION	 K8S VERSIONS
   *1.8.2    	tetrate	      0       	1.16,1.17,1.18
    1.8.1    	tetrate	      0       	1.16,1.17,1.18
    1.7.6    	tetrate	      0       	1.16,1.17,1.18
    1.7.5    	tetrate	      0       	1.16,1.17,1.18
    1.7.4    	tetrate	      0       	1.16,1.17,1.18

'*' indicates the currently active istioctl version.

The following is the explanation of each column:

[ISTIO VERSION]
The official tagged version of Istio on which the distribution is built.

[FLAVOR]
The kind of the distribution. As of now, there's one flavor which is called "tetrate",
and "tetratefips" flavor will be added shortly.

- "tetrate" flavor equals the official Istio except it is built by Tetrate.
- "tetratefips" flavor is FIPS-compliant, and can be used for installing FIPS-compliant control plain and data plain built by Tetrate.

[FLAVOR VERSION]
The flavor's version. A flavor version 0 maps to the distribution that is built on 
exactly the same source code of the corresponding official Istio version.

[K8S VERSIONS]
Supported k8s versions for the distribution

```

#### Options

```
  -h, --help   help for list
```

#### Options inherited from parent commands

```
  -c, --kubeconfig string   Kubernetes configuration file
```

#### SEE ALSO

* [getistio](/getistio-cli/reference/getistio/)	 - GetIstio is an integration and lifecycle management CLI tool that ensures the use of supported and trusted versions of Istio.

