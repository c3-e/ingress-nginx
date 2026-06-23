# Changelog

This file documents the C3-specific changes layered on top of upstream [ingress-nginx](https://github.com/kubernetes/ingress-nginx) Helm Chart 4.13.9 (controller v1.13.9). The release numbering uses [semantic versioning](http://semver.org).

### 4.13.9-c3.1

* Export controller health port via the service (PLAT-64979)
* Support private service connect (helm-chart-4.8.3-1)
* Remove pinned `digest`/`digestChroot` from the controller image so the C3 registry override (`registry.c3.ai/ingress-nginx-controller-fips`) takes effect
* Add `enableServiceLinks` support to the controller pod spec (Deployment and DaemonSet), defaulting to `false`

**Upstream base**: https://github.com/kubernetes/ingress-nginx/releases/tag/helm-chart-4.13.9
