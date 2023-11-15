# Adding Users to Groups

You'll need to use `usermod`.
To get help use:

```sh
man usermod
```

Try [searching](man.md) for `group` and `append`.

<details>

<summary>Solution</summary>

```sh
usermod -aG remote <USERNAME>
```

</details>
