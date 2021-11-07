docker build -t docker.example.com/dockeragent:latest .

docker push docker.example.com/dockeragent:latest

docker run -e AZP_URL=https://dev.azure.com/example -e AZP_TOKEN=abcdefghijklmnopqrstuvwxyz01234567890000000000000000 -e AZP_AGENT_NAME=mydockeragent docker.example.com/dockeragent:latest