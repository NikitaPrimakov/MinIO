# MinIO

```MinIO``` - is a High Performance Object Storage released under GNU Affero General Public License v3.0. It is API compatible with Amazon S3 cloud storage service.

## Resources

| Resource | Web-site |
| ------ | ------ |
| Documentation | https://min.io/docs/kes/ |
| GitHub | https://github.com/minio/minio |

## Deployment

In this part, we will look at the MinIO deployment process in a Kubernetes cluster.

To deploy the MinIO service in a local cluster, you need to describe several manifests:

- deployment-minio.yaml
- service-minio.yaml
- pvc-minio.yaml
- secrets-minio.yaml
- values.yaml

These files are located inside this project.
