# My Homelab
This is my humble attempt at infrastructure as code for my Proxmox server. The goal is to document all the Containers (and possibly VMs in the future) with their respective settings. 

> [!NOTE]
> This Repo is to be used with Ansible and Semaphore \
> use at your own risk :wink:

This repo goes along with my [homelab-ansible](https://github.com/mnul/homelab-ansible) repo for all the automation part in Ansible.

### ToDos
- [ ] Start with test-server
- [ ] Migrate currently running servers to the repo
- [ ] document how everything is laid out and how setup works

## Basic structure of the repo

The repo follows a basic structure

```
homelab/
├── servername/
│   ├── config/
│   │   └── main.yaml        # Public definition for server
│   └── files/              # Mirrors the root (/) of the server
│       └── docker/
│           ├── docker-compose.yaml
│           └── .env.example
└── servername2/
    ├── config/
    │   └── main.yaml
    └── files/
        └── ...
```
