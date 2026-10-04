# SSH Setup and Security

The Raspberry Pi was accessed remotely using SSH.

## Key-based authentication

Key-based SSH authentication was configured so that users could connect without entering a password.

The `.ssh` directory and `authorized_keys` file were checked to verify the setup.

## SSH hardening

The SSH configuration was then hardened by:

- disabling root login
- disabling password authentication
- allowing public-key authentication only
- restarting the SSH service
- verifying that the service was running correctly

A test user without key-based authentication was also used to confirm that password login was no longer accepted.

## Verification

Successful SSH connections were tested from multiple computers.
