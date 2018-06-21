Delete A Helm Release
---------------------
```bash
$ helm list --tiller-namespace=<NAMESPACE> | grep bluegreen | cut -f1 | xargs helm --tiller-namespace=<NAMESPACE> delete --purge
```
Thanks to https://stackoverflow.com/posts/47820015/revisions

Prepend String To Every File in Local Dir
-----------------------------------------
```
$ find *.* |  xargs -I{} mv {} rabbitmq-ha-{}
```
Inspiration from https://unix.stackexchange.com/questions/358613/prepend-to-filename-with-find-command
