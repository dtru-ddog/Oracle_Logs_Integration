# Service Connector Hub function
OCI function used for log forwarding. See [DataDog documentation for more info](https://docs.datadoghq.com/integrations/oracle_cloud_infrastructure/?tab=serviceconnectorhub#oci-function).

## Build
To build your Docker image you can do so via native Docker, or utilize OCIs built in CLI `fn` to build the resulting artifact (Note: Either method requires docker to be running).

Using `docker`:
```
docker image build -t dd-oci-object-store:latest .
```

Using `fn`:
```
fn build
```


## Tests

To run tests, cd into the current directory and run:

`python3 -m unittest`