# Requiring SSH Keys

![SSH Server Config](sshd-config.md)

Try searching for `Authentication`.

<detail>

<summary>Solution</summary>


```sh
nano /etc/ssh/sshd_config
```

Ensure these lines exists:

```
PasswordAuthentication no
KbdInteractiveAuthentication no
```

</detail>