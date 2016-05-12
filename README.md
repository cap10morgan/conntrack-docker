# conntrack-docker
Docker container for conntrack utility

## Usage

This will flush your ARP cache:

`docker run --net=host --privileged --rm cap10morgan/conntrack -F`

This is primarily used for working around Consul's tendency to use stale ARP entries when re-launched in Docker containers.
