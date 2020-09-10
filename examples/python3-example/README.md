# Python Example

## Build the Application

```
oc new-project myapp-python

oc new-app --name=python3-example python:3.6~https://gitlab.ar.bsch/santander-arq/vault-santander --context-dir=docs/integrations/examples/python3-example/
```

## Deploy
 
### Manual Sidecar Container

```
    oc apply -f examples/python3-example/python3-example.yaml
```

### Mutating Webhook Configuration

```
    oc apply -f examples/python3-example/python3-inject.yaml
```