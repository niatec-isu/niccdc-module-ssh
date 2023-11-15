# SCP

Use `scp`.
The syntax is very similar to `cp`.
To get help, use:

```sh
man scp
```

<details>

<summary>Solution</summary>

## Download (Server to Workstation)

```sh
scp <USERNAME>@<IP>:<FILE> .
```

## Upload (Workstation to Server)

```sh
scp <FILE> <USERNAME>@<IP>:.
```

</details>
