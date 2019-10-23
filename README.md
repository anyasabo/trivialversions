To demonstrate crd generation with trivial versions. Created with the tutorial using

```
kubebuilder init --domain tutorial.kubebuilder.io
kubebuilder create api --group batch --version v1 --kind CronJob
kubebuilder create api --group batch --version v2 --kind CronJob
```

and setting the marker

```
// +kubebuilder:storageversion
```

on the v2 object. The generated CRD with the trivial versions option is stored in `./config/crd/bases`
