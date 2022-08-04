# Ansible Role: WSDD

Basic role to install and confiure WSDD on Ubuntu or Debian from https://github.com/christgau/wsdd

Role parameters:

| parameter         | description                                                                               | default                           |
| ----------------- | ----------------------------------------------------------------------------------------- | --------------------------------- |
| wsdd_git_url      | Repository URL to clone from                                                              | https://github.com/christgau/wsdd |
| wsdd_version      | Repository version to use (e.g. `HEAD` or a SHA)                                          | `HEAD`                            |
| wsdd_download_dir | Local directory to clone the repository. The repository will be left for tracking changes | `/tmp/wsdd`                       |
| wsdd_params       | Parameters to pass to wsdd. Refer to the wsdd manpage for arguments.                      | `--shortlog`                      |
| install_ufw_rule  | Whether to install a ufw rule for wsdd and enable it.                                     | `false`                           |
