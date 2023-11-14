Use `nano` to edit the SSH server config:

```sh
sudo nano /etc/ssh/sshd_config
```

Once you've saved the file and closed nano, restart the SSH server:

```sh
sudo systemctl restart sshd
```
Use `man` to see the available options:

```sh
man sshd_config
```

[man](man.md)
