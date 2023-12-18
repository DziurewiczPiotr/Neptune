# Neptune

## SSH connection

`If you didn't already`
SSH keys should be generated on the computer you wish to log in from

```
ssh-keygen -t rsa
ssh-copy-id {remote_host}
ssh -p {port_number} {remote_host}
```

## Commands

- `podman build -t neptune_nginx .`
- `podman run -d -p 8080:80 neptune_nginx`
- `podman attach --latest`
- `podman exec -it --latest bash`
- `podman run -d -p 4200:4200 --network=host neptune_prefect_server`


## Danger Zone

- `podman system prune -a`
