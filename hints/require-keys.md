# Requiring SSH Keys

[SSH Server Config](sshd-config.md)

Try [searching](hints/man.md) for `Authentication` in `man sshd_config`.

<details>

<summary>Solution</summary>


```sh
nano /etc/ssh/sshd_config
```

Ensure these lines exists:

```
PasswordAuthentication no
KbdInteractiveAuthentication no
```

</details>
