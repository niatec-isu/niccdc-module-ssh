# Disable Root Login Through SSH

[SSH Server Config](sshd-config.md)

Try [searching](hints/man.md) for `Root` in `man sshd_config`.

<details>

<summary>Solution</summary>


```sh
nano /etc/ssh/sshd_config
```

Ensure this line exists:

```
PermitRootLogin no
```

</details>
