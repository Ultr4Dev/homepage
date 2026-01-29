# No explanation needed

## Docker Image

This project automatically builds and publishes a Docker image to GitHub Container Registry (ghcr.io) when changes are pushed to the main branch.

### Accessing the Published Image

Pull the latest image:
```bash
docker pull ghcr.io/ultr4dev/homepage:latest
```

Or pull a specific commit (replace `abc1234` with the actual commit SHA):
```bash
docker pull ghcr.io/ultr4dev/homepage:main-abc1234
```

### Running the Container

```bash
docker run -p 8080:80 ghcr.io/ultr4dev/homepage:latest
```

Then visit http://localhost:8080 in your browser.
