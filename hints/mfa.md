# SSH MFA

![SSH Server Config](sshd-config.md)

Try searching for `Authentication`.

<detail>

<summary>Solution</summary>


```sh
nano /etc/ssh/sshd_config
```

Ensure these lines exists:

```
PasswordAuthentication yes
AuthenticationMethods publickey,password
```

</detail>