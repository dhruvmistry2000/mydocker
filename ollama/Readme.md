## Hosting Local AI with Ollama

<span><img src="https://raw.githubusercontent.com/loganmarchione/homelab-svg-assets/c378f0a492cacfa327b9cc7b4b97fa6605f72de8/assets/ollama-white.svg" alt="Ollama Logo" width="50" height="50" /></span>
<span><img src="https://docs.openwebui.com/images/logo.png" alt="OWUI Logo" width="50" height="50" /></span>

This Docker Compose file sets up a local environment for hosting Large Language Models (LLMs) using Ollama and OpenWebUI. Below are the steps to use this Docker Compose file.

### Benefits of Running AI Locally
1. **Enhanced Privacy:** Running AI models locally ensures that your data remains on your own hardware, reducing the risk of data breaches and maintaining confidentiality.
2. **Reduced Latency:** Local hosting minimizes the time taken for data to travel to and from remote servers, resulting in faster response times and improved performance for AI applications.

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
