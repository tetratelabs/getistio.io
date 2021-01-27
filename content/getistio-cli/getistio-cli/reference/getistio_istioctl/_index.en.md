---
title: "getistio istioctl"
url: /getistio-cli/reference/getistio_istioctl/
---
## getistio istioctl

Execute istioctl with given arguments

#### Synopsis

Execute istioctl with given arguments where the version of istioctl is specified at ~/.getistio/config.json.

```
getistio istioctl <args...> [flags]
```

#### Examples

```
# install istio with the default profile
getistio istioctl install --set profile=default

# check versions of istio data plane, control plane, and istioctl
getistio istioctl version
```

#### Options

```
  -h, --help   help for istioctl
```

#### Options inherited from parent commands

```
  -c, --kubeconfig string   Kubernetes configuration file
```

#### SEE ALSO

* [getistio](/getistio-cli/reference/getistio/)	 - GetIstio is an integration and lifecycle management CLI tool that ensures the use of supported and trusted versions of Istio.

