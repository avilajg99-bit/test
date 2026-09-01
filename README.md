# test

## Connect your servers

Use SSH to connect to each server with your own hostnames, usernames, and key paths:

```bash
ssh user@server-1.example.com
ssh user@server-2.example.com
```

For repeated access, add entries like these to `~/.ssh/config`:

```sshconfig
Host server-1
  HostName server-1.example.com
  User your-user
  IdentityFile ~/.ssh/your-key

Host server-2
  HostName server-2.example.com
  User your-user
  IdentityFile ~/.ssh/your-key
```

Then connect with:

```bash
ssh server-1
ssh server-2
```

Do not commit private keys, passwords, or other secrets to this repository.