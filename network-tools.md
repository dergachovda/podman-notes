# Running Container with Network Tools

Run a container with network tools:

```bash
podman run -it --rm --cap-add=NET_RAW busybox
```

### With Root
By default, Podman runs containers as root.

### Without Root
To run without root, add `--user 1000` (or another non-root user ID) to the command:

```bash
podman run -it --rm --cap-add=NET_RAW --user 1000 busybox
```

## Related Articles
- [BusyBox Official Documentation - Network Tools](https://busybox.net/downloads/BusyBox.html)
- [Linux.com Networking Topic - Practical Guides](https://www.linux.com/topic/networking/)
- [Podman Container Networking Documentation](https://docs.podman.io/en/latest/)