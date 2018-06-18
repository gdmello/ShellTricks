Delete A Helm Release
=====================
```bash
$ helm list --tiller-namespace=<NAMESPACE> | grep bluegreen | cut -f1 | xargs helm --tiller-namespace=<NAMESPACE> delete --purge
```
Thanks to https://stackoverflow.com/posts/47820015/revisions
