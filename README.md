# Docmost Deploy - Ansible

# For staging

`ansible-playbook -i inventory.yml site.yml --limit staging`

# For production

`ansible-playbook -i inventory.yml site.yml --limit production`

# Directory structure

```
.
├── README.md
├── docker-compose.yml
├── inventory.yml
├── roles
│   └── docmost
│   ├── defaults
│   │   └── main.yml
│   ├── handlers
│   │   └── main.yml
│   ├── meta
│   │   └── main.yml
│   ├── tasks
│   │   ├── config.yml
│   │   ├── docker.yml
│   │   ├── healthcheck.yml
│   │   ├── main.yml
│   │   ├── packages.yml
│   │   ├── service.yml
│   │   └── setup.yml
│   └── templates
│   ├── docker-compose.yml.j2
│   ├── dockmost.service.j2
│   ├── docmost-logrotate.j2
│   └── nginx.conf.j2
└── site.yml
```
