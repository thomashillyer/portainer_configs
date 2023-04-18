# portainer_configs
collection of dockerfiles and docker compose files that are used in my local homelab portainer setup

infra_compose.yml is the compose file that lives directly on the server. It contains adguard and portainer configuration.
networking_compose.yml is for tailscale. It isn't used, but is for future reference.
homeassistant_compose.yml is for homeassistant and associated containers (basically everything stable)
eufy_compose.yml is for testing new containers for a eufy integration. It may move to homeassistant containers once stable.

Run the only local compose file:
`docker compose -f infra_compose.yml up -d`
