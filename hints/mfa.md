# SSH MFA

[SSH Server Config](sshd-config.md)

Try [searching](man.md) for `Authentication` in `man sshd_config`.

<details>

<summary>Solution</summary>


```sh
nano /etc/ssh/sshd_config
```

Ensure these lines exists:

```
PasswordAuthentication yes
AuthenticationMethods publickey,password
```

</details>
