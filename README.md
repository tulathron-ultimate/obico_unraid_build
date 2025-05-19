# Unraid Obico Docker Image

  This repository builds a Docker image for running the [Obico server](https://github.com/TheSpaghettiDetective/obico-server) on Unraid. It is based on the official `thespaghettidetective/obico-server:release` image and configured for Unraid compatibility.

  ## Usage
  - **Docker Hub Image**: `docker.io/tulathron/unraid-obico:latest`
  - **Unraid Installation**:
    1. Use the provided Unraid template (`unraid-obico-template.xml`) in Unraid’s Docker tab.
    2. Pull the image from `docker.io/tulathron/unraid-obico`.
    3. Configure ports, volumes, and environment variables as needed.
  - **Access**: Open `http://<your-unraid-ip>:3334` and log in with `root@example.com`/`supersecret` (change password immediately).

  ## Building Locally
  ```bash
  docker build -t tulathron/unraid-obico:latest .
  ```

  ## Notes
  - This image uses CPU-based AI detection by default to avoid CUDA dependencies.
  - For GPU support, install the Unraid Nvidia Driver plugin and add `--gpus all` to Extra Parameters.
  - See [Obico documentation](https://www.obico.io/docs/server-guides/) for setup details.

  ## Repository
  - GitHub: [tulathron-ultimate/obico_unraid_build](https://github.com/tulathron-ultimate/obico_unraid_build)
  - Docker Hub: [tulathron/unraid-obico](https://hub.docker.com/r/tulathron/unraid-obico)

  ## License
  AGPL-3.0, matching the [Obico server license](https://github.com/TheSpaghettiDetective/obico-server/blob/master/LICENSE).