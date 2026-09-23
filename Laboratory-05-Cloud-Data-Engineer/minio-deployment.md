# MinIO Deployment

## Docker Command

The MinIO server was deployed using Docker with the following command:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
quay.io/minio/minio server /data --console-address ":9001"
```

## Web Console Port

The MinIO Web Console was accessed using port **9001** through the KillerCoda Traffic Port Accessor.

## Bucket Created

The storage bucket created for the project is:

**client-photos**

## Environment Variables

The `-e` flags in the Docker command are used to set environment variables for the MinIO container.

- `MINIO_ROOT_USER=cloudadmin` sets the MinIO administrator username.
- `MINIO_ROOT_PASSWORD=CloudNova2026!` sets the MinIO administrator password.

These environment variables provide the login credentials used to access the MinIO Web Console.
