# Build Proxmox Templates via Packer
Pass the proxmox `root` password via the `PROXMOX_PWD` environment variable at the command prompt

####  Build Ubuntu 18.04 template
```shell
PROXMOX_PWD=XXXXXXXXXXX packer build ubuntu_18.04.json
```

####  Build Ubuntu 20.04 template
```shell
PROXMOX_PWD=XXXXXXXXXXX packer build ubuntu_20.04.json
```

#### Requirements
- To be run at **PROXMOX** server
- Ensure `packer` is installed
- Ensure ISO files specified under `variables`.`iso_filename` are present under folder `/var/lib/vz/templates/iso`
