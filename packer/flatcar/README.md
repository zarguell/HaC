# Configuration

To generate the ignition.json for flatcar install, run:

```
ct -pretty -in-file flatcar-linux-config.yml -out-file ignition.json
```

(Dependent on ct utility: https://github.com/coreos/container-linux-config-transpiler)

Above utility is deprecated, possibly better alternative:

```
cat cl.yaml | docker run --rm -i ghcr.io/flatcar-linux/ct:latest > ignition.json
```
