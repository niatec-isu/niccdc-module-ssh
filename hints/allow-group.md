# Allowing Groups

[SSH Server Config](sshd-config.md)

Try [searching](man.md) for `Group` in `man sshd_config`.

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
