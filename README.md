# nft-safe-reload

Reload nftables configuration and wait for user confirmation.
After a timeout the previous configuration is restored.
This should help prevent admins from locking themselves out of a system.

Original Author: https://sanjuroe.dev/nft-safe-reload

This version containes proper shell quoting.

## The new nftables configuration has to be confirmed

```
# nft-safe-reload 
Do you want to accept the new firewall configuration? [y/n] y
Accepted new configuration
```

## If you cannot confirm it, the previous configuration will be loaded again

```
# nft-safe-reload 
Do you want to accept the new firewall configuration? [y/n] Restored old configuration
```

