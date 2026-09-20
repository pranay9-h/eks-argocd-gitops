# Security

## Repository rules

Never commit:

- AWS credentials
- kubeconfig files
- private keys
- container registry passwords
- GitHub personal access tokens
- Argo CD admin passwords
- Kubernetes Secret manifests containing real secret values

## Kubernetes security controls demonstrated

- non-root pod execution
- RuntimeDefault seccomp profile
- dropped Linux capabilities
- privilege escalation disabled
- read-only root filesystem
- resource requests and limits
- health probes

## Secret handling

This portfolio intentionally does not store real application secrets. In a real platform, use an approved secrets manager and a Kubernetes integration such as External Secrets Operator or the cloud provider's supported secret-delivery mechanism.
