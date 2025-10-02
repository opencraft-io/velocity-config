# Velocity Config

This repository contains the configuration files required to deploy Velocity proxies for the different environments (`dev`, `staging`, `prod`).

Each environment includes:  
- `velocity.toml`: main Velocity configuration.  
- `forwarding.secret`: secret used for forwarding between the proxy and Minecraft servers.

## Dependencies

- Kubernetes deployment of the proxies: [minecraft-proxies](https://github.com/opencraft-io/minecraft-proxies)  

## Notes

- The `forwarding.secret` files are sensitive. They will soon be stored in **HashiCorp Vault** and removed from this repository.