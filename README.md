# Ansible Automation Project

This repository contains a collection of Ansible playbooks that automate various tasks, including server provisioning and configuration management.

## Project Structure

```
.
├── README.md
├── inventory
│   ├── production
│   └── staging
├── group_vars
│   ├── all.yml
│   ├── webservers.yml
│   └── dbservers.yml
├── host_vars
│   └── example-host.yml
├── roles
│   ├── common
│   ├── webserver
│   └── database
└── playbooks
    ├── site.yml
    ├── webserver.yml
    └── database.yml
```

## Playbooks

- `site.yml`: Main playbook that includes all other playbooks
- `webserver.yml`: Playbook for configuring web servers
- `database.yml`: Playbook for configuring database servers

## Roles

- `common`: Common tasks for all servers
- `webserver`: Tasks specific to web servers
- `database`: Tasks specific to database servers

## Usage

1. Update the inventory files with your server information.
2. Modify the group_vars and host_vars as needed.
3. Run the playbooks using the `ansible-playbook` command:

```
ansible-playbook -i inventory/production playbooks/site.yml
```

## Author

Kumbirai Muhwati

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.