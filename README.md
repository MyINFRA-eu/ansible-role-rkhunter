# MyINFRA.eu Ansible Role: RKHunter

[![MyINFRA.eu logo](https://raw.githubusercontent.com/MyINFRA-eu/.github/main/logo/myinfra-logo-grey.svg)](https://myinfra.eu)


## About

A little description about the project.


## Support us

We invest a lot of resources and time into creating these ansible roles. You can supports us by [sponsoring this project](https://github.com/MyINFRA-eu#sponsorship).

We highly appreciate you mentioning us or our projects on you website, social media, ...


## Statistics

**Releases**

![GitHub Release](https://img.shields.io/github/v/release/MyINFRA-eu/ansible-role-rkhunter?style=flat)
![GitHub Release Date](https://img.shields.io/github/release-date/MyINFRA-eu/ansible-role-rkhunter?style=flat)
![GitHub Downloads (all assets, all releases)](https://img.shields.io/github/downloads/MyINFRA-eu/ansible-role-rkhunter/total?style=flat)
![GitHub Downloads (all assets, latest release)](https://img.shields.io/github/downloads/MyINFRA-eu/ansible-role-rkhunter/latest/total?style=flat)

**Commits/Activity**

![GitHub branch status](https://img.shields.io/github/checks-status/MyINFRA-eu/ansible-role-rkhunter/main?style=flat)
![GitHub last commit](https://img.shields.io/github/last-commit/MyINFRA-eu/ansible-role-rkhunter?style=for-the-badge?style=flat)
![GitHub commit activity](https://img.shields.io/github/commit-activity/w/MyINFRA-eu/ansible-role-rkhunter?style=flat)
![GitHub commits since latest release](https://img.shields.io/github/commits-since/MyINFRA-eu/ansible-role-rkhunter/latest?style=flat)
![GitHub contributors](https://img.shields.io/github/contributors/MyINFRA-eu/ansible-role-rkhunter?style=for-the-badge?style=flat)

**Repository**

![GitHub repo file or directory count](https://img.shields.io/github/directory-file-count/MyINFRA-eu/ansible-role-rkhunter?style=flat)
![GitHub repo size](https://img.shields.io/github/repo-size/MyINFRA-eu/ansible-role-rkhunter?style=flat)
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/MyINFRA-eu/aansible-role-rkhunter?style=flat)
![GitHub language count](https://img.shields.io/github/languages/count/MyINFRA-eu/ansible-role-rkhunter?style=flat)
![GitHub top language](https://img.shields.io/github/languages/top/MyINFRA-eu/ansible-role-rkhunter?style=flat)

**Ansible Galaxy**

![Ansible Collection Version](https://img.shields.io/ansible/collection/v/myinfra_eu/rkhunter?style=flat)
![Ansible Collection Downloads](https://img.shields.io/ansible/collection/d/myinfra_eu/rkhunter?style=flat)
![Ansible Role](https://img.shields.io/ansible/role/d/myinfra_eu/rkhunter?style=flat)

**Owner**

![GitHub Sponsors](https://img.shields.io/github/sponsors/Dennis-de-Houx?style=for-the-badge)
![GitHub followers](https://img.shields.io/github/followers/Dennis-de-Houx?style=for-the-badge)
![GitHub User's stars](https://img.shields.io/github/stars/Dennis-de-Houx?style=for-the-badge)

**Organisation**

![GitHub Org's stars](https://img.shields.io/github/stars/MyINFRA-eu?style=for-the-badge)


## Requirements

None.


## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

### install

Install rkhunter and run rkhunter

> value needs to be a boolean (true|false)

```yml
rkhunter
  install: true
```

### cron

Install crontab script to be run every day

> value needs to be a boolean (true|false)

```yml
rkhunter
  cron: true
```

### path

Define a custom path for your config files if you don't want to use your default ones.

```yml
rkhunter
  path: "/opt/custom/storage"
```


## Dependencies

None.


## Example Playbook

```
- hosts: all
  vars_files:
    - vars/main.yml
  roles:
    - { role: myinfra_eu.rkhunter }
```


## Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information on what has changed recently.


## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for details.


## Security Vulnerabilities

Please review [our security policy](https://github.com/MyINFRA-eu/ansible-role-rkhunter/security/policy) on how to report security vulnerabilities.


## Credits

- [Dennis de houx](https://github.com/Dennis-de-Houx)
- [All Contributors](https://github.com/MyINFRA-eu/ansible-role-rkhunter/contributors)


## Copyright

- (c) 2025 MyINFRA.eu ~ [https://myinfra.eu](https://myinfra.eu)
- (c) 2025 All In One ~ [https://all-in-one.be](https://all-in-one.be)
- (c) 2025 Dennis de houx ~ [https://dehoux.be](https://dehoux.be)


## Inspiration

During development some roles in Ansible Galaxy/Github also inspired me,
thanks to the following developers for the inspiration:

- [geerlingguy](https://github.com/geerlingguy/)


## License

The Attribution-NonCommercial-NoDerivatives 4.0 International License. Please see [License File](LICENSE.md) for more information.
