# images

Recipes for the golden VM images that [Opifica](https://github.com/opifica) workers boot for each job.

Each organisation builds its own images from these recipes. Images are signed and hashed, and workers refuse to
boot an image whose hash doesn't match. Opifica does not distribute prebuilt Windows or macOS images; licensing
for those operating systems stays with the organisation running them.

> **Status:** early development.

| Path | Guest OS | Hypervisor |
|---|---|---|
| `linux/` | Linux | Firecracker |
| `windows/` | Windows | Hyper-V |
| `macos/` | macOS | Apple Virtualization.framework (Apple hardware only, max. 2 VMs per Mac) |

## Stack

Packer · the Opifica agent baked into every image

## License

[EUPL-1.2](LICENSE)
