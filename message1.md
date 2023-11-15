# First Message

Hey team,

We need your help securing our SSH server.
To access the server, you'll need to log into your workstation.
Once in, open a terminal and use [SSH](hints/ssh.md) to access the server at 10.0.0.227.
You'll be using the username `john` and password `ILovePineappl3`.

We've noticed that several users are logging in with root through SSH.
We'd like to [disable this](hints/disable-root-ssh.md), as this violates company policy.

We'd also like to improve our overall security posture.
Users are currently logging in using passwords, which leaves us vulnerable to brute forcing attacks.
We'd like to require the use of SSH keys.
This will need to be done in multiple steps.
You'll need to [generate](hints/ssh-keygen.md) an `ed25519` key for yourself on your workstation.
Then you'll need to [copy your key](hints/ssh-copy-id.md) to the SSH server, as well as [manually copy](hints/manual-copy.md) the attached keys to the appropriate user accounts.
At this point, you should [disable both](hints/require-keys.md) password authentication and keyboard interactive authentication.
You should also take the time to [remove](hints/remove-keys.md) any other authorized keys that you didn't copy over, as they are rogue keys.
While removing them, just delete the line that contains the key, not the file itself.

Thanks team!
When you're done, we have [another task](message2.md) for you.

## Attachments

- [Jacob's Key](keys/jacob_ed25519.pub)
- [Jingleheimer's Key](keys/jingleheimer_ed25519.pub)
- [Schmidt's Key](keys/schmidt_ed25519.pub)
