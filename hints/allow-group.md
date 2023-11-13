# Allowing Groups

![SSH Server Config](sshd-config.md)

Try searching for `Group`.

<detail>

<summary>Solution</summary>


```sh
nano /etc/ssh/sshd_config
```

Ensure this line exists:

```
AllowGroups remote
```

</detail>