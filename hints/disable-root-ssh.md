# Disable Root Login Through SSH

![SSH Server Config](sshd-config.md)

Try searching for `Root`.

<detail>

<summary>Solution</summary>


```sh
nano /etc/ssh/sshd_config
```

Ensure this line exists:

```
PermitRootLogin no
```

</detail>