# Remove Authorized Keys

There are several rogue keys on this server.
To remove them, you'll need to check each users `~/.ssh/authorized_keys` file.
When removing rogue keys, don't delete the `authorized_keys` file, just delete the line containing the rogue key.

<detail>

<summary>Solution</summary>

```sh
sudo su
nano /home/maleficent/.ssh/authorized_keys
nano /home/rumpelstiltskin/.ssh/authorized_keys
```

Remove the rogue keys from the two files.

</detail>
