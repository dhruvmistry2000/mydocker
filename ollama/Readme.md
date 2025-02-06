## Dockerfile for Ollama

<span><img src="https://raw.githubusercontent.com/loganmarchione/homelab-svg-assets/c378f0a492cacfa327b9cc7b4b97fa6605f72de8/assets/ollama-white.svg" alt="Ollama Logo" width="50" height="50" /></span>
<span><img src="https://docs.openwebui.com/images/logo.png" alt="OWUI Logo" width="50" height="50" /></span>



### Running Docker Compose for CPU and GPU
To run the Docker Compose files for CPU and GPU, follow these instructions:

1. **For CPU:**
   - Navigate to the directory containing the `docker-compose-cpu.yml` file.
   - Run the following command to start the CPU services:

     ```bash
     docker-compose -f docker-compose-cpu.yml up
     ```

2. **For GPU:**
   - Navigate to the directory containing the `docker-compose-gpu.yml` file.
   - Run the following command to start the GPU services:

     ```bash
     docker-compose -f docker-compose-gpu.yml up
     ```

This will create and start the necessary containers for both CPU and GPU environments.
