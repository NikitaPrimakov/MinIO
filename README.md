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

1. We need to create a namespace in which the application will be deployed.

```
kubectl create ns minio
```

Using the 

```
kubectl get ns command
```
 we can check

![kubectl get ns](https://github.com/NikitaPrimakov/MinIO/blob/e5aa4953bcbeefcd2c1269a643be5d3cf13aa92e/kubectl%20get%20ns.png "kubectl get ns")

The next step is to deploy MinIO.

1. Using git, we will clone this project.

2. Using the ```kubectl apply -f ./<name of manifest>``` command, we will deploy our service. If necessary, make changes to these manifests according to your requirements.

3. The result will be the web interface of the MinIO application.

