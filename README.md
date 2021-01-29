# Dependencies

Scripts are written in fish and require rg (ripgrep) to work.

```shell
apt-get install fish ripgrep
```

`fish --version` must be >= 3.1.0  

Put `concordium-client` in /usr/local/bin/

# Install

1. For all four challenge-ot4-t* scripts you'll need the list of receivers.  

Receive will be picked randomly for each transaction.

```shell
concordium-client account list > accounts-list.txt
```

> WARNING: Remove your account(s) from accounts-list.txt before proceed

2. Copy all fish scripts and accounts-list.txt to ~/scripts

See [crontab.example.sh](crontab.example.sh) for how to config your crontab.  
Replace `<user>`, `<passwod>` and `<sender>` with real values.