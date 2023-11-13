# NICCDC Module: SSH

| #   | Pre | Challenge                   | Evaluation                                                  |
| --- | --- | --------------------------- | ----------------------------------------------------------- |
| M   | N/A | First Message               | N/A                                                         |
| 1   | N/A | Disable root SSH access     | `/etc/ssh/sshd_config` for `PermitRootLogin no`             |
| 2   | N/A | Generate and copy keys      | Check `~/.ssh/authorized_keys` for users                    |
| 3   | N/A | Require the use of SSH keys | `/etc/ssh/sshd_config` for `PasswordAuthentication no`      |
| 4   | N/A | Remove unknown SSH keys     | `~/.ssh/authorized_keys` for no extra keys                  |
| M   | 1-4 | Second Message              | N/A                                                         |
| 5   | 1-4 | Add users to `remote` group | Check if authorized users are in the remote group           |
| 6   | 1-4 | Whitelist `remote` group    | `/etc/ssh/sshd_config` for `AllowGroups remote`             |
| M   | 5-6 | Third Message               | N/A                                                         |
| 7   | 5-6 | Implement some form of MFA  | `sshd_config` for `PassAuth yes` and `AuthMeth pubkey,pass` |

## Messages

- [First Message](message1.md)
- [Second Message](message2.md)
- [Third Message](message3.md)
