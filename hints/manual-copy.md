# Copying Others' SSH Keys

## Hint 1

You will need to [SSH](ssh.md) into the server.
Run `sudo su` to become a root.
Then use `nano` to edit the user's authorized keys file, copying and pasting their key.

## Hint 2

You will first need to copy the key to the server with [SCP](scp.md).
You will need to [SSH](ssh.md) into the server.
Run `sudo su` to become a root.
Then cat the key and redirect it to it's user's authorized keys file.

<detail>

<summary>Solution</summary>

## Solution 1

```sh
ssh <YOUR_USERNAME>@<IP>
sudo su
nano /home/<OTHER_USERNAME>/.ssh/authorized_keys
```

Once in the file, copy and paste the key, then save with `Ctrl+S` and exit with `Ctrl+X`

## Solution 2

```sh
scp <OTHER_USERNAME>_ed25519.pub <YOUR_USERNAME>@<IP>:.
ssh <YOUR_USERNAME>@<IP>
sudo su
cat <OTHER_USERNAME>_ed25519.pub >> /home/<OTHER_USERNAME>/.ssh/authorized_keys
```

</detail>