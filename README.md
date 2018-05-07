# Sojobo Bundles
This repository contains three juju bundles that will setup a Sojobo-environment. Currently we support 3 cloud-types: Aws, GCE and Azure.
After deploying the prefered bundle a few more steps will have to be taken to completely setup your environment.

### Google GCE Bundle
```
juju config sojobo-api cloud-region="europe-west1"
juju config sojobo-api cloud-credential="{'private_key_id': xxx, 'client_id': xxxx, 'token_uri': xxx, 'auth_uri': xxxx, 'type': xxxx, 'auth_provider_x509_cert_url': xxxx, 'client_x509_cert_url': xxx, 'client_email': xxx, 'private_key': xxxx, 'project_id': xxx}"
```

### AWS Bundle
```
juju config sojobo-api cloud-region="eu-west-1"
juju config sojobo-api cloud-credential="{'access-key': xxxxx, 'secret-key': xxx}"
```

### Azure Bundle
```
juju config sojobo-api cloud-region="northeurope"
juju config sojobo-api cloud-credential="{'application-id': xxxx, 'application-password': xxxx, 'subscription-id': xxx}"
```

## Contact Information
- Sebastien Pattyn <sebastien.pattyn@tengu.io>
