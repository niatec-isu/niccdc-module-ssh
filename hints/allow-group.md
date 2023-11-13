# Allowing Groups

![SSH Server Config](sshd-config.md)

Try searching for `Group`.

<details>

<summary>Solution</summary>


```sh
nano /etc/ssh/sshd_config
```

Ensure this line exists:

```
AllowGroups remote
```

</details>