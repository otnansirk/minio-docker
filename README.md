# MinIO Docker Project

This project provides a simple setup for running [MinIO](https://min.io/) using Docker Compose. MinIO is a high-performance, S3 compatible object storage service.

## Project Structure

```
docker-compose.yml
```

- `docker-compose.yml`: Docker Compose file to set up and run MinIO.
- `minio-data/`: Directory where MinIO stores its data.

## Usage

### Prerequisites
- [Docker](https://www.docker.com/get-started)
- [Docker Compose](https://docs.docker.com/compose/)

### Running MinIO

1. Clone this repository:
   ```sh
   git clone git@github.com:otnansirk/minio-docker.git
   cd minio-docker
   ```
2. Start MinIO using Docker Compose:
   ```sh
   docker-compose up -d
   ```
3. Access the MinIO Console:
   - Open your browser and go to: [http://localhost:9001](http://localhost:9001)
   - Default credentials (unless changed in `docker-compose.yml`):
     - **Username:** minioadmin
     - **Password:** minioadmin

### Stopping MinIO

To stop the MinIO server:
```sh
docker-compose down
```

## Data Persistence

All uploaded files and buckets are stored in the `minio-data/` directory. This ensures your data persists across container restarts.

## License

This project is open source and available under the [MIT License](LICENSE).
