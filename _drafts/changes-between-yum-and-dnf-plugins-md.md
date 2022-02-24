---
title: changes-between-yum-and-dnf-plugins.md
author:
  name: Johan Sörell
  link: 
categories: [Linux ]
tags: [Linux, dnf, yum, plugins]
---



# Changes between YUM and DNF plugins


|                                       |                                                                                                                |                                  |
| ------------------------------------- | -------------------------------------------------------------------------------------------------------------- | -------------------------------- |
| Original YUM tool                     | DNF command/option                                                                                             | Package                          |
| `yum check`                           | [dnf repoquery](https://dnf.readthedocs.io/en/latest/command_ref.html#repoquery-command-label) `--unsatisfied` | `dnf`                            |
| `yum-langpacks`                       |                                                                                                                | `dnf`                            |
| `yum-plugin-aliases`                  | [dnf alias](https://dnf.readthedocs.io/en/latest/command_ref.html#alias-command-label)                         | `dnf`                            |
| `yum-plugin-auto-update-debug-info`   | option in `debuginfo-install.conf`                                                                             | `dnf-plugins-core`               |
| `yum-plugin-changelog`                |                                                                                                                | `dnf-plugins-core`               |
| `yum-plugin-copr`                     | [dnf copr](https://dnf-plugins-core.readthedocs.io/en/latest/copr.html)                                        | `dnf-plugins-core`               |
| `yum-plugin-fastestmirror`            | `fastestmirror` option in [dnf.conf](https://dnf.readthedocs.io/en/latest/conf_ref.html)                       | `dnf`                            |
| `yum-plugin-fs-snapshot`              |                                                                                                                | `dnf-plugins-extras-snapper`     |
| `yum-plugin-local`                    |                                                                                                                | `dnf-plugins-core`               |
| `yum-plugin-merge-conf`               |                                                                                                                | `dnf-plugins-extras-rpmconf`     |
| `yum-plugin-post-transaction-actions` |                                                                                                                | `dnf-plugins-core`               |
| `yum-plugin-priorities`               | `priority` option in [dnf.conf](https://dnf.readthedocs.io/en/latest/conf_ref.html)                            | `dnf`                            |
| `yum-plugin-remove-with-leaves`       | [dnf autoremove](https://dnf.readthedocs.io/en/latest/command_ref.html#autoremove-command-label)               | `dnf`                            |
| `yum-plugin-show-leaves`              |                                                                                                                | `dnf-plugins-core`               |
| `yum-plugin-tmprepo`                  | `--repofrompath` option                                                                                        | `dnf`                            |
| `yum-plugin-tsflags`                  | `tsflags` option in [dnf.conf](https://dnf.readthedocs.io/en/latest/conf_ref.html)                             | `dnf`                            |
| `yum-plugin-versionlock`              |                                                                                                                | `python3-dnf-plugin-versionlock` |
| `yum-rhn-plugin`                      |                                                                                                                | `dnf-plugin-spacewalk`           |

