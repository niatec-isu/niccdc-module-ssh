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

There are links in each message that act as hints.
Feel free to use the hints as much as you'd like,
but try to solve this without looking at the solutions!

- [First Message](message1.md)
- [Second Message](message2.md)
- [Third Message](message3.md)

## Connecting

The Workstation VM is currently hosted on Proxmox, and is only accessible from the NIATEC lab.
Access it by visiting https://192.168.33.111:8006/#v1:0:=qemu%2F118:4:5:=contentIso:::8::5,
using `root` as the username, and the password from STACHE.

**The username and password are in the [first message](message1.md).**

If you are not automatically connected to the VM, use these steps to connect.
The VM is on `pve-r430-4` and is called `riley-ssh-workstation`.
Click on the VM, then on Console near the top-left of the screen.
