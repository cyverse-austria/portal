# portal

CyVerse user portal kustomiz


## Usage

To deploy this kustomize, clone the repository and follow the below steps.

### change the domain in nginx

replace the `your-domain.com` in file [base\nginx.conf](base\nginx.conf) with your portal domain name.

### add your secrets

Fill in the secrets in file [base\kustomization.yaml](base\kustomization.yaml).

### apply

```bash
kubectl apply -k /base -n $namespace
```
